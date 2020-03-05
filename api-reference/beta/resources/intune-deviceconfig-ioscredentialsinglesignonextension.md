---
title: Тип ресурса Иоскредентиалсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с использованием учетных данных для устройств с iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b661c7a5fb94216efdc20b8e6474d9cbec6d5883
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529947"
---
# <a name="ioscredentialsinglesignonextension-resource-type"></a>Тип ресурса Иоскредентиалсинглесигнонекстенсион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль расширения единого входа с использованием учетных данных для устройств с iOS.


Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|екстенсионидентифиер|String|Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|теамидентифиер|String|Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|домена|Коллекция String|Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.|
|область|String|Получает или задает имя области для этого профиля, заданное с учетом регистра.|
|построения|Коллекция [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)|Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCredentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```



