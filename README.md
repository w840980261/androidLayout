# androidLayout

```
<LinearLayout
        android:layout_width="361dp"
        android:layout_height="229dp"
        android:orientation="vertical"
        tools:layout_editor_absoluteX="-1dp"
        tools:layout_editor_absoluteY="8dp">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="50dp"
            android:orientation="horizontal">

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="One,One"
                android:textAllCaps="false"
                android:textSize="12sp"  />

            <Button
                android:layout_width="120dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="One,Two"
                android:textAllCaps="false"
                android:textSize="12sp"  />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="One,Three"
                android:textAllCaps="false"
                android:textSize="12sp"  />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="One,Four"
                android:textAllCaps="false"
                android:textSize="12sp" />
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="50dp"
            android:orientation="horizontal">

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Two,One"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="120dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Two,Two"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Two,Three"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Two,Four"
                android:textAllCaps="false"
                android:textSize="12sp" />
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="50dp"
            android:orientation="horizontal">

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Three,One"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Three,Two"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Three,Three"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Three,Four"
                android:textAllCaps="false"
                android:textSize="12sp" />
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="50dp"
            android:orientation="horizontal">

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Four,One"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="120dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Four,Two"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Four,Three"
                android:textAllCaps="false"
                android:textSize="12sp" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Four,Four"
                android:textAllCaps="false"
                android:textSize="12sp" />
        </LinearLayout>
    </LinearLayout>
```
效果图：

![image](https://raw.githubusercontent.com/w840980261/androidLayout/master/img/1.png)

```
<android.support.constraint.ConstraintLayout
        android:layout_width="362dp"
        android:layout_height="204dp"
        tools:ignore="MissingConstraints"
        tools:layout_editor_absoluteX="0dp"
        tools:layout_editor_absoluteY="0dp">


        <Button
            android:id="@+id/button1"
            android:layout_width="80dp"
            android:layout_height="50dp"
            android:layout_weight="1"
            android:background="#f00"
            android:gravity="center"
            android:text="red"
            app:layout_constraintHorizontal_chainStyle="spread_inside"
            app:layout_constraintLeft_toLeftOf="parent"
            app:layout_constraintRight_toLeftOf="@+id/button2" />

        <Button
            android:id="@+id/button2"
            android:layout_width="80dp"
            android:layout_height="50dp"
            android:layout_weight="1"
            android:background="#ffa600"
            android:gravity="center"
            android:text="orange"
            app:layout_constraintLeft_toRightOf="@+id/button1"
            app:layout_constraintRight_toLeftOf="@+id/button3" />

        <Button
            android:id="@+id/button3"
            android:layout_width="80dp"
            android:layout_height="50dp"
            android:layout_weight="1"
            android:background="#ffff00"
            android:gravity="center"
            android:text="yellow"
            app:layout_constraintLeft_toRightOf="@+id/button2"
            app:layout_constraintRight_toRightOf="parent" />


        <Button
            android:id="@+id/button4"
            android:layout_width="70dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#0f0"
            android:gravity="center"
            android:text="green"
            app:layout_constraintHorizontal_chainStyle="packed"
            app:layout_constraintLeft_toLeftOf="parent"
            app:layout_constraintRight_toLeftOf="@+id/button5"
            app:layout_constraintTop_toBottomOf="@+id/button1" />

        <Button
            android:id="@+id/button5"
            android:layout_width="70dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#0000ff"
            android:gravity="center"
            android:text="blue"
            app:layout_constraintLeft_toRightOf="@+id/button4"
            app:layout_constraintRight_toLeftOf="@+id/button6"
            app:layout_constraintTop_toBottomOf="@+id/button1" />

        <Button
            android:id="@+id/button6"
            android:layout_width="70dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#4a0084"
            android:gravity="center"
            android:text="indigo"
            app:layout_constraintLeft_toRightOf="@+id/button5"
            app:layout_constraintRight_toRightOf="parent"
            app:layout_constraintTop_toBottomOf="@+id/button1" />

        <Button
            android:layout_width="0dip"
            android:layout_height="50dp"
            android:layout_marginTop="10dp"
            android:layout_weight="1"
            android:background="#ef82ef"
            android:gravity="center"
            android:text="violet"
            app:layout_constraintLeft_toLeftOf="parent"
            app:layout_constraintRight_toRightOf="parent"
            app:layout_constraintTop_toBottomOf="@+id/button5" />
    </android.support.constraint.ConstraintLayout>
```
效果图：

![image](https://raw.githubusercontent.com/w840980261/androidLayout/master/img/2.png)

```
<TableLayout
        android:layout_width="365dp"
        android:layout_height="495dp"
        tools:layout_editor_absoluteX="0dp"
        tools:layout_editor_absoluteY="0dp"
        android:stretchColumns="1"
        android:shrinkColumns="2"
        android:background="#fff"
        >

        <TableRow
            android:layout_width="match_parent"
            android:layout_height="match_parent" >

            <TextView
                android:layout_width="20dp"
                android:layout_height="wrap_content"
                android:paddingLeft="5dp"
                android:text="" />
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Open..." />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:paddingRight="10dp"
                android:text="Ctrl-O"
                android:textAlignment="viewEnd" />
        </TableRow>

        <TableRow
            android:layout_width="match_parent"
            android:layout_height="match_parent" >

            <TextView
                android:layout_width="20dp"
                android:layout_height="wrap_content"
                android:paddingLeft="5dp"
                android:text="" />
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Save..." />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:paddingRight="10dp"
                android:text="Ctrl-S"
                android:textAlignment="viewEnd" />
        </TableRow>

        <TableRow
            android:layout_width="match_parent"
            android:layout_height="match_parent" >

            <TextView
                android:layout_width="20dp"
                android:layout_height="wrap_content"
                android:paddingLeft="5dp"
                android:text="" />
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Save As..." />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:paddingRight="10dp"
                android:text="Ctrl-Shift-S"
                android:textAlignment="viewEnd" />
        </TableRow>

        <TableRow
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:background="#666">

            <TextView
                android:layout_width="20dp"
                android:layout_height="wrap_content"
                android:paddingLeft="5dp"
                android:text="X"
                android:background="#fff"
                android:layout_marginTop="1dp"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="1dp"
                android:text="Import..."
                android:background="#fff"/>

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="1dp"
                android:background="#fff"
                android:paddingRight="10dp"
                android:text=""
                android:textAlignment="viewEnd" />
        </TableRow>

        <TableRow
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:background="#666" >

            <TextView
                android:layout_width="20dp"
                android:layout_height="wrap_content"
                android:paddingLeft="5dp"
                android:text="X"
                android:background="#fff"
                android:layout_marginBottom="1dp"/>
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Export..."
                android:background="#fff"
                android:layout_marginBottom="1dp"/>

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginBottom="1dp"
                android:background="#fff"
                android:paddingRight="10dp"
                android:text="Ctrl-E"
                android:textAlignment="viewEnd" />
        </TableRow>

        <TableRow
            android:layout_width="match_parent"
            android:layout_height="match_parent" >

            <TextView
                android:layout_width="20dp"
                android:layout_height="wrap_content"
                android:paddingLeft="5dp"
                android:text="" />
            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Quit..." />

        </TableRow>
    </TableLayout>
```
效果图：

![image](https://raw.githubusercontent.com/w840980261/androidLayout/master/img/3.png)