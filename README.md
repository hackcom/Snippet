# C#
### How to change XML self closing tag to full end tag.
inputXml.DescendantNodes().OfType<XElement>().Where(x => x.IsEmpty).ToList().ForEach(x => x.Value = string.Empty);
