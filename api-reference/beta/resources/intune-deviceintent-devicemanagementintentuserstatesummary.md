---
title: тип ресурса deviceManagementIntentUserStateSummary
description: Объект, представляю который представляет сводку состояния пользователя для намерения
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 37b7ce6567d2000a453cd2c1ca45e6be5b340edf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091477"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a>тип ресурса deviceManagementIntentUserStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляю который представляет сводку состояния пользователя для намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Чтение свойств и связей [объекта deviceManagementIntentUserStateSummary.](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|
|[Обновление deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Обновление свойств объекта [deviceManagementIntentUserStateSummary.](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|The ID|
|conflictCount|Int32|Количество пользователей в конфликте|
|errorCount|Int32|Число пользователей ошибок|
|failedCount|Int32|Число сбойных пользователей|
|notApplicableCount|Int32|Число не применимых пользователей|
|successCount|Int32|Число пользователей, успешно успешно|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```



