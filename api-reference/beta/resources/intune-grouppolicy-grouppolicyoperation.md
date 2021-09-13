---
title: тип ресурса groupPolicyOperation
description: Объект представляет операцию групповой политики.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad6ee2f261c14a4a1ad7548561ac6487d2745223
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086101"
---
# <a name="grouppolicyoperation-resource-type"></a>тип ресурса groupPolicyOperation

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет операцию групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyOperations](../api/intune-grouppolicy-grouppolicyoperation-list.md)|[коллекция groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Список свойств и связей объектов [groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|
|[Get groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-get.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Чтение свойств и связей объекта [groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|
|[Создание groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-create.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Создайте новый [объект groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|
|[Удаление groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-delete.md)|Нет|Удаляет [группуPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).|
|[Обновление groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-update.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Обновление свойств объекта [groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operationType|[groupPolicyOperationType](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|Тип операции групповой политики. Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|operationStatus|[groupPolicyOperationStatus](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|Состояние операции групповой политики. Возможные значения: `unknown`, `inProgress`, `success`, `failed`.|
|statusDetails|String|Подробное состояние состояния операции групповой политики.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "String",
  "operationStatus": "String",
  "statusDetails": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



