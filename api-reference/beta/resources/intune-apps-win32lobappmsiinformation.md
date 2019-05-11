---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd612a5593ef151d4f324f3058c793ce7cd29bf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949635"
---
# <a name="win32lobappmsiinformation-resource-type"></a>Тип ресурса win32LobAppMsiInformation

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства приложения MSI для приложения Win32.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|productCode|Строка|Код продукта MSI.|
|productVersion|Строка|Версия продукта MSI.|
|upgradeCode|Строка|Код обновления MSI.|
|Рекуиресребут|Логический|Требует ли приложение MSI перезагрузку компьютера для завершения установки.|
|Паккажетипе|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|Тип пакета MSI. Возможные значения: `perMachine`, `perUser`, `dualPurpose`.|
|productName|String|Имя продукта MSI.|
|publisher|Строка|Издатель MSI.|

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




