---
title: Тип ресурса Редиректсинглесигнонекстенсион
description: Представляет расширение Apple Single Sign-On.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b899a0bfcb80c57bdfc889a4a857950678946c6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198222"
---
# <a name="redirectsinglesignonextension-resource-type"></a>Тип ресурса Редиректсинглесигнонекстенсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет расширение Apple Single Sign-On.


Наследуется от [синглесигнонекстенсион](../resources/intune-deviceconfig-singlesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|екстенсионидентифиер|String|Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|теамидентифиер|String|Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|построения|Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)|Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|
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




