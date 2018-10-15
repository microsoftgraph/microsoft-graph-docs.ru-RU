# <a name="organization-resource-type"></a>Тип ресурса organization

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс organization представляет экземпляр глобальных параметров и ресурсов, которые действуют и готовятся в работе на уровне клиента.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список организаций](../api/intune_onboarding_organization_list.md)|Коллекция объектов [organization](../resources/intune_onboarding_organization.md)|Список свойств и связей объектов [organization](../resources/intune_onboarding_organization.md).|
|[Получение организации](../api/intune_onboarding_organization_get.md)|[организация](../resources/intune_onboarding_organization.md)|Чтение свойств и связей объекта [organization](../resources/intune_onboarding_organization.md).|
|[Обновление организации](../api/intune_onboarding_organization_update.md)|[организация](../resources/intune_onboarding_organization.md)|Обновление свойств объекта [organization](../resources/intune_onboarding_organization.md).|
|[Действие setMobileDeviceManagementAuthority](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|Int32|Задание центра управления мобильными устройствами|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ид|Строка|GUID объекта.|
|mobileDeviceManagementAuthority|[mdmAuthority](../resources/intune_onboarding_mdmauthority.md)|Центр управления мобильными устройствами. Возможные значения: `unknown`, `intune`, `sccm`, `office365`.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->






