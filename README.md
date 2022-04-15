namespace WinFormsApp4

{
    public partial class Form1 : materialform

    {
        readonly MaterialSkin.MaterialSkinManager materialSkinManager;
        public Form1()
        {
            InitializeComponent();
            materialSkinManager = MaterialSkin.MaterialSkinManager.Instance;
            materialSkinManager.EnforceBackcolorOnAllComponents = true;
            materialSkinManager.AddFormToManage(this);
            materialSkinManager.Theme = MaterialSkin.MaterialSkinManager.Themes.LIGHT;
            materialSkinManager.ColorScheme = new MaterialSkin.ColorScheme(MaterialSkin.Primary.Teal900, MaterialSkin.Primary.Cyan900, MaterialSkin.Primary.Teal700, MaterialSkin.Accent.Cyan700, MaterialSkin.TextShade.WHITE);
        }
    }

    public class materialform
    { }
}

