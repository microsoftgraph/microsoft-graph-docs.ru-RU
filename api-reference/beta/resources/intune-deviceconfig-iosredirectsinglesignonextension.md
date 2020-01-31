---
title: Тип ресурса Иосредиректсинглесигнонекстенсион
description: Представляет профиль расширения единого входа с перенаправлением для устройств с iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85048bbbdf66166a053be93a124653b17d680a21
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636695"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a>Тип ресурса Иосредиректсинглесигнонекстенсион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль расширения единого входа с перенаправлением для устройств с iOS.


Наследуется от [иоссинглесигнонекстенсион](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|екстенсионидентифиер|Строка|Получает или задает идентификатор пакета расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|теамидентифиер|Строка|Получает или задает идентификатор группы расширения приложения, выполняющего единый вход для указанных URL-адресов.|
|построения|Коллекция [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)|Получает или задает список типизированных пар "ключ — значение", используемых для настройки профилей типа учетных данных. Эта коллекция может содержать не более 500 элементов.|
|урлпрефиксес|Коллекция String|Один или несколько префиксов URL-адресов поставщиков удостоверений, у которых расширение приложения выполняет единый вход. URL-адреса должны начинаться с http://или https://. Все префиксы URL-адреса должны быть уникальными для всех профилей.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosRedirectSingleSignOnExtension",
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



