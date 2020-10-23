---
title: Тип ресурса Андроидманажедстореапптракк
description: Содержит сведения о записях для приложений управляемого хранилища Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab4009dfb8fc6cfd40ae49529e07a6a6932d7c4d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690275"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a>Тип ресурса Андроидманажедстореапптракк

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит сведения о записях для приложений управляемого хранилища Android.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|траккид|Строка|Уникальный идентификатор записи.|
|траккалиас|Строка|Понятное имя для отслеживания.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppTrack"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppTrack",
  "trackId": "String",
  "trackAlias": "String"
}
```





