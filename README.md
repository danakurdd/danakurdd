  private void Form1_Load(object sender, EventArgs e)
  {
      LoadData();
      foreach (SkinContainer cn in SkinManager .Default.Skins)
      {
          comboBoxEdit1.Properties.Items.Add(cn.SkinName);

      }
  }
          private void comboBoxEdit1_SelectedIndexChanged(object sender, EventArgs e)
        {
            DevExpress.LookAndFeel.UserLookAndFeel.Default.SetSkinStyle(comboBoxEdit1.Text);
        }
