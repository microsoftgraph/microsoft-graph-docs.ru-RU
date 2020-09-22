---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение единого входа Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 348f6c194c1084bf186812cb4e86edba8b9b7579
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049585"
---
# <a name="redirectsinglesignonextension-resource-type"></a>Тип ресурса Редиректсинглесигнонекстенсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет расширение единого входа Apple.


Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|екстенсионидентифиер|Строка|Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|теамидентифиер|Строка|Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|построения|Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)|Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|
|урлпрефиксес|Коллекция String|Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход. URL-адреса должны начинаться с http://или https://. Все префиксы URL-адреса должны быть уникальными для всех профилей.|

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






