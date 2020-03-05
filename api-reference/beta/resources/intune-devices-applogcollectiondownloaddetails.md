---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc54ac6e98634f641408590b122cd69246e24044
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528711"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a>Тип ресурса Апплогколлектиондовнлоаддетаилс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|довнлоадурл|String|Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест|
|декриптионкэй|String|Декриптионкэй как строка|
|appLogDecryptionAlgorithm|[appLogDecryptionAlgorithm](../resources/intune-devices-applogdecryptionalgorithm.md)|Декриптионалгорисм для контента. Возможные значения: `aes256`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```



