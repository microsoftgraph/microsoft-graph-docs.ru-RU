    ---
Заголовок: описание «educationIdentitySynchronizationConfiguration ресурсов типа»: «абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций. Производные классы определите поведение синхронизации удостоверения. Ниже приведены производных типов.»
Автор: «mmast-msft» localization_priority: обычный ms.prod: «education»
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>Тип ресурса educationIdentitySynchronizationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций. Производные классы определите поведение синхронизации удостоверения. Ниже приведены производные типы.

## <a name="derived-types"></a>Производные типы
| Тип | Описание |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Этот тип используется в соответствии с существующим учетным записям пользователей в Azure Active Directory (Azure AD). |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Этот тип используется для создания новых учетных записей пользователей в Azure AD. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
