# Documenta-o-WPF
Documentação que contêm explicação de Classes, Controles, Lógicas e manipulações do WPF
<hr>

## Canvas
Canvas é útil quando você precisa posicionar elementos em posições XY fixas na tela. É mais simples e prático do que usar as "Correntes" do Visual Studio 2022.

```xml
<Canvas>
    <Button Canvas.Left="50" Canvas.Top="30" Content="Clique Aqui"/>
    <TextBlock Canvas.Left="100" Canvas.Top="100" Text="Texto Posicionado"/>
</Canvas>
```

## ComboBox
ComboBox é uma lista suspensa de opções que permite ao usuário escolher entre os itens dentro do ComboBox.

```xml
<ComboBox>
    <ComboBoxItem Content="Opção 1"/>
    <ComboBoxItem Content="Opção 2"/>
    <ComboBoxItem Content="Opção 3"/>
</ComboBox>
```

## Label e TextBlock
- **Label**: Usado para descrever controles, como um TextBox, já que o Label pode ser associado a outros elementos.
- **TextBlock**: Usado para escrever informações "soltas" que não estão diretamente relacionadas a outro elemento.

```xml
<Label Content="Nome:" Target="{Binding ElementName=txtNome}"/>
<TextBox Name="txtNome"/>
<TextBlock Text="Texto exibido aqui"/>
```

## ListBox
Semelhante ao ComboBox, mas não é uma lista suspensa. Dependendo da configuração, permite a seleção de múltiplos itens.

```xml
<ListBox>
    <ListBoxItem Content="Item 1"/>
    <ListBoxItem Content="Item 2"/>
    <ListBoxItem Content="Item 3"/>
</ListBox>
```

## StackPanel
StackPanel é usado para organizar elementos, como botões, vertical ou horizontalmente.

```xml
<StackPanel Orientation="Vertical">
    <Button Content="Botão 1"/>
    <Button Content="Botão 2"/>
    <Button Content="Botão 3"/>
</StackPanel>
```

## TabControl
TabControl permite criar abas para separar o conteúdo de forma lógica e organizada.

```xml
<TabControl>
    <TabItem Header="Aba 1">
        <TextBlock Text="Conteúdo da Aba 1"/>
    </TabItem>
    <TabItem Header="Aba 2">
        <TextBlock Text="Conteúdo da Aba 2"/>
    </TabItem>
</TabControl>
```

## DockPanel
DockPanel organiza a estrutura XAML de forma mais simples, ancorando elementos nas bordas do programa.

```xml
<DockPanel>
    <Button Content="Topo" DockPanel.Dock="Top"/>
    <Button Content="Esquerda" DockPanel.Dock="Left"/>
    <Button Content="Direita" DockPanel.Dock="Right"/>
    <Button Content="Preenche o Resto"/>
</DockPanel>
```

## Expander
Expander permite expandir e colapsar seu conteúdo, economizando espaço na interface.

```xml
<Expander Header="Mais Detalhes">
    <TextBlock Text="Aqui estão os detalhes"/>
</Expander>
```

## Frame
Frame é utilizado para exibir diferentes páginas de conteúdo ou navegação dentro de uma aplicação.

```xml
<Frame Source="PaginaInicial.xaml"/>
```

## Cursor
A propriedade `Cursor` define como o ponteiro do mouse deve se comportar ao passar sobre um elemento XAML.

```xml
<Button Content="Clique Aqui" Cursor="Hand"/>
```
