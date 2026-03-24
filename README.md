# android-studio-arthur

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#FFFFFF"
    tools:context=".MainActivity">


    <TextView
        android:id="@+id/textview_title"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginLeft="20dp"
        android:layout_marginTop="32dp"
        android:gravity="center"
        android:text="CALCULADORA IMC"
        android:textSize="40sp"
        android:textStyle="bold"
        android:textColor="#000000"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <EditText
        android:id="@+id/edit_text_peso"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="36dp"
        android:layout_marginEnd="16dp"
        android:hint="Peso"
        android:textSize="20sp"
        android:textColor="#000000"
        android:textColorHint="#808080"
        android:backgroundTint="#000000"
        app:layout_constraintTop_toBottomOf="@id/textview_title"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent"/>

    <TextView
        android:id="@+id/textview_altura"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="32dp"
        android:text="Altura (cm)"
        android:textSize="20sp"
        android:textColor="#000000"
        app:layout_constraintTop_toBottomOf="@id/edit_text_peso"
        app:layout_constraintStart_toStartOf="parent"/>

    <TextView
        android:id="@+id/textview_resultado"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="40dp"
        android:text="IMC: 0.0"
        android:textSize="28sp"
        android:textStyle="bold"
        android:textColor="#000000"
        android:visibility="gone"
        app:layout_constraintTop_toBottomOf="@id/textview_Altura"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />
    <SeekBar
        android:id="@+id/seekbar_altura"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="16dp"
        android:layout_marginEnd="16dp"
        android:max="250"
        android:min="0"
        android:progressTint="#000000"
        android:progressBackgroundTint="#000000"
        app:layout_constraintTop_toBottomOf="@id/textview_altura"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent"/>

    <TextView
        android:id="@+id/textview_Altura"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="8dp"
        android:text="180 cm"
        android:textColor="#000000"
        app:layout_constraintTop_toBottomOf="@id/seekbar_altura"
        app:layout_constraintStart_toStartOf="parent"/>

    <Button
        android:id="@+id/button_limpar"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="140dp"
        android:text="Limpar"
        android:textSize="22sp"
        android:backgroundTint="#55ba05"
        android:textColor="#000000"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toStartOf="@id/button_calcular" />

    <Button
        android:id="@+id/button_calcular"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="140dp"
        android:text="Calcular"
        android:textSize="22sp"
        android:backgroundTint="#55ba05"
        android:textColor="#000000"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toEndOf="@id/button_limpar"
        app:layout_constraintEnd_toEndOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
