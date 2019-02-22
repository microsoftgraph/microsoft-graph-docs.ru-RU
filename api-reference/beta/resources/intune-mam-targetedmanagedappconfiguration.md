---
title: Тип ресурса targetedManagedAppConfiguration
description: Конфигурация, используемая для предоставления набора настраиваемых параметров в исходном виде для всех пользователей в целевой группе безопасности.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6adafe694a7abb55cd64a5fbfbd64e3c66b7e6e4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149240"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a>Тип ресурса targetedManagedAppConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация, используемая для предоставления набора настраиваемых параметров в исходном виде для всех пользователей в целевой группе безопасности.


Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-list.md)|Коллекция объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Получение объекта targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md);|Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Создание объекта targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md);|Создание объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Удаление объекта targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|Нет|Удаление объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Обновление объекта targetedManagedAppConfiguration](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).|
|[Действие assign](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|None|Н/Д|
|[Действие targetApps](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|None|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Ключ объекта. Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|version|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|customSettings|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).|
|deployedAppCount|Int32|Количество приложений, для которых развернута текущая политика.|
|isAssigned|Логический|Указывает, применена ли политика к группам включения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
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




