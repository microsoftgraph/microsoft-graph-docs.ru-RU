---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 13d8ec94fafd3ae571278a62cd2e331c7f07886d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725549"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a>Тип ресурса Апплогколлектиондовнлоаддетаилс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|довнлоадурл|Строка|Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест|
|декриптионкэй|Строка|Декриптионкэй как строка|
|appLogDecryptionAlgorithm|[appLogDecryptionAlgorithm](../resources/intune-devices-applogdecryptionalgorithm.md)|Декриптионалгорисм для контента. Возможные значения: `aes256` .|

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





