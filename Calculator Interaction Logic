using System.Windows;
using System.Windows.Input;


namespace Calculator
{
    /// <summary>
    /// Interaction logic for MainWindow.xaml
    /// </summary>
    public partial class MainWindow : Window
    {
        float num1 = 0;
        float num2 = 0;
        float result = 0;
        string operation = "";

        public MainWindow()
        {
            InitializeComponent();
            
        }
           
        private void Window_MouseDown(object sender, System.Windows.Input.MouseButtonEventArgs e)
        {
            try
            {
                this.DragMove();

            }
            catch 
            {

                
            }
        }
    
        //NUMBERS

        private void btn1_Click(object sender, RoutedEventArgs e)
        {
            if(operation == "")
            {
                num1 = (num1 * 10) + 1;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
               
                num2 = (num2 * 10) + 1;
                txtDisplayer.Text = num2.ToString();
            }
         
        }

        private void btn2_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 2;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 2;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn3_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 3;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 3;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn4_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 4;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 4;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn5_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 5;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 5;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn6_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 6;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 6;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn7_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 7;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 7;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn8_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 8;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 8;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn9_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10) + 9;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10) + 9;
                txtDisplayer.Text = num2.ToString();
            }
        }

        private void btn0_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 = (num1 * 10);
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 = (num2 * 10);
                txtDisplayer.Text = num2.ToString();
            }
        }


        
        //Matth Operations
        private void btnplus_Click(object sender, RoutedEventArgs e)
        {                      
            operation = "+";
            PlusCalculateandDisplay();
        }

        private void btnminus_Click(object sender, RoutedEventArgs e)
        {
            operation = "-";
            MinusCalculateandDisplay();
        }

        private void btnX_Click(object sender, RoutedEventArgs e)
        {
            operation = "x";
            MultiplieCalculateandDisplay();
        }

        private void btnDivide_Click(object sender, RoutedEventArgs e)
        {
            operation = "/";
            DivideCalculateandDisplay();
        }

        private void btnEQ_Click(object sender, RoutedEventArgs e)
        {
           if(operation == "+")
            {
                PlusCalculateandDisplay();
            }
           else if(operation == "-")
            {
                MinusCalculateandDisplay();
            }
           else if (operation == "x")
            {
                MultiplieCalculateandDisplay();
            }
           else if (operation == "/")
            {
                DivideCalculateandDisplay();
            }
        }

        //Support Buttons

        private void btnCE_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
                num1 = 0;
            else
                num2 = 0;
            txtDisplayer.Text = "0";
   
        }

        private void btnC_Click(object sender, RoutedEventArgs e)
        {
            num1 = 0;
            num2 = 0;

            operation = "";
            txtDisplayer.Text = "0";
            txtCalculateDisplayer.Text = "0";
        }

        private void btnDel_Click(object sender, RoutedEventArgs e)
        {
            txtDisplayer.Text.Remove(txtDisplayer.Text.Length - 1);
           
        }

        private void btnPosNev_Click(object sender, RoutedEventArgs e)
        {
            if (operation == "")
            {
                num1 *= -1;
                txtDisplayer.Text = num1.ToString();
            }
            else
            {
                num2 *= -1;
                txtDisplayer.Text = num2.ToString();
            }
        }

        //Methods


        private void CloseCommandHandlers(object sender, ExecutedRoutedEventArgs e)
        {
            this.Close();
        }

        private void PlusCalculateandDisplay()
        {
            result = num1 + num2;
            txtDisplayer.Text = (num1 + num2).ToString();
            txtCalculateDisplayer.Text = result.ToString() + " " + operation;

            num1 = result;
            num2 = 0;
        }

        private void MinusCalculateandDisplay()
        {
            result = num1 - num2;
            txtDisplayer.Text = (num1 - num2).ToString();
            txtCalculateDisplayer.Text = result.ToString() + " " + operation;

            num1 = result;
            num2 = 0;
        }

        private void MultiplieCalculateandDisplay()
        {
            if (num2 == 0)
                result = num1;
            else
                result = num1 * num2;
            txtDisplayer.Text = result.ToString();
            txtCalculateDisplayer.Text = num1.ToString() + " " + operation;

            num1 = result;
            num2 = 0;
        }

        private void DivideCalculateandDisplay()
        {
            if (num2 == 0)
                result = num1;
            else
                result = num1 / num2;
            txtDisplayer.Text = result.ToString();
            txtCalculateDisplayer.Text = num1.ToString() + " " + operation;

            num1 = result;
            num2 = 0;
        }
    }
