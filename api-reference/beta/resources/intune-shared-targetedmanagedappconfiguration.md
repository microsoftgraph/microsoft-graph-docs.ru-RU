---
title: Тип ресурса targetedManagedAppConfiguration
description: Конфигурация, используемая для предоставления набора настраиваемых параметров в исходном виде для всех пользователей в целевой группе безопасности.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 651ea39e6134626a7086909d6b4807eaa37a32a2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449621"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a>Тип ресурса targetedManagedAppConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация, используемая для предоставления набора настраиваемых параметров в исходном виде для всех пользователей в целевой группе безопасности.


Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-list.md)|Коллекция объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Получение объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md);|Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Создание объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md);|Создание объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Удаление объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|Нет|Удаление объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Обновление объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|**Управление мобильным приложением (MAM)**|
|[Действие assign](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|None|Н/Д|
|[Действие targetApps](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|None|Н/Д|
|**Набор политик**|
|[действие Хаспайлоадлинкс](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов областей для этого экземпляра сущности. Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|customSettings|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).|
|deployedAppCount|Int32|Количество приложений, для которых развернута текущая политика.|
|isAssigned|Boolean|Указывает, применена ли политика к группам включения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление мобильным приложением (MAM)**|
|apps|Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Список приложений, к которым применена политика.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Свойства навигации к сводке по развертыванию конфигурации.|
|assignments|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Список групп включения и исключения, к которым применяется политика.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```



