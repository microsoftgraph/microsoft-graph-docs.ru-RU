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

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

