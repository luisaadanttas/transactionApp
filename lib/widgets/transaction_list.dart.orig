import 'package:flutter/material.dart';
import 'package:intl/intl.dart';
import '../models/transaction.dart';

class TransactionList extends StatelessWidget {
  final List<Transaction> transactions;
  final Function deleteTx;

  TransactionList(this.transactions, this.deleteTx);
  @override
  Widget build(BuildContext context) {
<<<<<<< HEAD
    return transactions.isEmpty
        ? Column(
            children: <Widget>[
              Text(('No Transactions added yet!'),
                  style: Theme.of(context).textTheme.headline6),
              SizedBox(height: 10),
              Container(
                height: 200,
                child: Image.asset(
                  'assets/images/waiting.png',
                  fit: BoxFit.cover,
=======
    return Container(
      height: 450,
      child: transactions.isEmpty
          ? Column(
              children: <Widget>[
                Text(('No Transactions added yet!'),
                    style: Theme.of(context).textTheme.headline6),
                SizedBox(height: 10),
                Container(
                  height: 200,
                  child: Image.asset(
                    'assets/images/waiting.png',
                    fit: BoxFit.cover,
                  ),
>>>>>>> 9156402b1e151123496f418afab4506836df2e27
                ),
              ),
            ],
          )
        : ListView.builder(
            itemBuilder: (ctx, index) {
              return Card(
                elevation: 5,
                margin: EdgeInsets.symmetric(vertical: 8, horizontal: 5),
                child: ListTile(
                  leading: CircleAvatar(
                    radius: 30,
                    child: Padding(
                      padding: EdgeInsets.all(6),
                      child: FittedBox(
                          child: Text('\$${transactions[index].amount}')),
                    ),
<<<<<<< HEAD
=======
                    subtitle: Text(
                        DateFormat.yMMMd().format(transactions[index].date)),
                    trailing: IconButton(
                      icon: Icon(Icons.delete),
                      color: Theme.of(context).errorColor,
                      onPressed: () => deleteTx(transactions[index].id),
                    ),
>>>>>>> 9156402b1e151123496f418afab4506836df2e27
                  ),
                  title: Text(
                    transactions[index].title,
                    style: Theme.of(context).textTheme.headline6,
                  ),
                  subtitle:
                      Text(DateFormat.yMMMd().format(transactions[index].date)),
                ),
              );
            },
            itemCount: transactions.length,
          );
  }
}
