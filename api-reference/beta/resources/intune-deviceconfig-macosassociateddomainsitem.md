---
title: Тип ресурса МакосассоЦиатеддомаинситем
description: Сопоставление идентификаторов приложений со связанными доменами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b14cc5fe7c13bbcdde94733c41caf2b68c0451e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268939"
---
# <a name="macosassociateddomainsitem-resource-type"></a>Тип ресурса МакосассоЦиатеддомаинситем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление идентификаторов приложений со связанными доменами.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationIdentifier|String|Идентификатор приложения, с которым связываются домены.|
|домена|Коллекция строк|Список подсвязываемых доменов.|
|директдовнлоадсенаблед|Boolean|Определяет, будут ли данные загружаться напрямую или с помощью сети CDN.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsItem",
  "applicationIdentifier": "String",
  "domains": [
    "String"
  ],
  "directDownloadsEnabled": true
}
```




