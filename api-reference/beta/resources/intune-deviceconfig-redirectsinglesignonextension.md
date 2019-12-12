---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение единого входа Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a408d9cfd364f222ad87fd3796d7037ed51ab76a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955527"
---
# <a name="redirectsinglesignonextension-resource-type"></a>Тип ресурса Редиректсинглесигнонекстенсион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет расширение единого входа Apple.


Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|екстенсионидентифиер|Строка|Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|теамидентифиер|Строка|Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|построения|Коллекция [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)|Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|
|урлпрефиксес|Коллекция строк|Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход. URL-адреса должны начинаться с http://или https://. Все префиксы URL-адреса должны быть уникальными для всех профилей.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.redirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.redirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



