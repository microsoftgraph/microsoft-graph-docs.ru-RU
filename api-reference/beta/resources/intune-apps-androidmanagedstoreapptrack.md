---
title: тип ресурса AndroidManagedStoreAppTrack
description: Содержит сведения о отслеживании для приложений Управляемого магазина Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 73d33337049b83c50d18c4274b71331a7483d12d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819740"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a>тип ресурса AndroidManagedStoreAppTrack

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит сведения о отслеживании для приложений Управляемого магазина Android.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|trackId|String|Уникальный идентификатор дорожки.|
|trackAlias|String|Удобное имя для трека.|

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



