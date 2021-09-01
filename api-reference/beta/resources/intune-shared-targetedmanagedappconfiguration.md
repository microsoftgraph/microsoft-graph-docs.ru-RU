---
title: Тип ресурса targetedManagedAppConfiguration
description: Конфигурация, используемая для предоставления набора настраиваемых параметров в исходном виде для всех пользователей в целевой группе безопасности.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3042e46a41a8282e3d4392365fcc6f2cc7e035e2
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786931"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a>Тип ресурса targetedManagedAppConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация, используемая для предоставления набора настраиваемых параметров в исходном виде для всех пользователей в целевой группе безопасности.


Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-list.md)|Коллекция объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Получение объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Создание объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Создание объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Удаление объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|Нет|Удаление объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|[Обновление объекта targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).|
|**Управление мобильным приложением (MAM)**|
|[Действие assign](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|Нет|Н/Д|
|[Действие targetApps](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|Нет|Н/Д|
|**Набор политик**|
|[действие hasPayloadLinks](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
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



