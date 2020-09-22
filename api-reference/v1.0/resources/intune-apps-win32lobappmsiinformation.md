---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a812789a8231731b171edea8e15f7f540266cbde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080166"
---
# <a name="win32lobappmsiinformation-resource-type"></a>Тип ресурса win32LobAppMsiInformation

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства приложения MSI для приложения Win32.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|productCode|String|Код продукта MSI.|
|productVersion|String|Версия продукта MSI.|
|upgradeCode|Строка|Код обновления MSI.|
|рекуиресребут|Boolean|Требует ли приложение MSI перезагрузку компьютера для завершения установки.|
|паккажетипе|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|Тип пакета MSI. Возможные значения: `perMachine`, `perUser`, `dualPurpose`.|
|productName|String|Имя продукта MSI.|
|publisher|String|Издатель MSI.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```





