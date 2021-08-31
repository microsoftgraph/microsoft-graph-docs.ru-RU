---
title: тип ресурса windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Класс, содержащий свойства, используемые для Политики Windows10EnrollmentCompletionPageConfiguration PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0995358cc2a877dc6fe6b2c799c997326408850a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803218"
---
# <a name="windows10enrollmentcompletionpageconfigurationpolicysetitem-resource-type"></a>тип ресурса windows10EnrollmentCompletionPageConfigurationPolicySetItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для Политики Windows10EnrollmentCompletionPageConfiguration PolicySetItem.


Наследует от [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10EnrollmentCompletionPageConfigurationPolicySetItems](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-list.md)|[коллекция windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Список свойств и связей объектов [Windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|
|[Get windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-get.md)|[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Чтение свойств и связей [объекта Windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|
|[Создание windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-create.md)|[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Создайте [новый объект Windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|
|[Удаление windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-delete.md)|Нет|Удаляет [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md).|
|[Обновление windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-update.md)|[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Обновление свойств объекта [Windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Клавиша PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время политикиSetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|Строка|PayloadId of the PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|Строка|policySetType policySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName of the PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние PolicySetItem. Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки, если таковое произошло. Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Коллекция String|Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)|
|priority|Int32|Приоритет Windows10EnrollmentCompletionPageConfigurationPolicySetItem.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "priority": 1024
}
```



