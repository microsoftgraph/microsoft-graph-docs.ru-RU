    ---
Title: "Едукатионидентитисинчронизатионконфигуратион типа ресурса" Описание: "абстрактный базовый класс для всех конфигураций синхронизации удостоверений профилей учебных данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: "ммаст — MSFT" локализатион_приорити: Normal MS. произ: "образование"
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>Тип ресурса Едукатионидентитисинчронизатионконфигуратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.

## <a name="derived-types"></a>ПроизВодные типы
| Тип | Описание |
|:-|:-|
| [**Едукатионидентитиматчингконфигуратион**](educationidentitymatchingconfiguration.md) | Используйте этот тип для согласования с существующими учетными записями пользователей в Azure Active Directory (Azure AD). |
| [**Едукатионидентитикреатионконфигуратион**](educationidentitycreationconfiguration.md) | Используйте этот тип для создания новых учетных записей пользователей в Azure AD. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
