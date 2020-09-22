---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6206dbc62fa8ae9ff0dee4d47bec30ce4ae99ae0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003642"
---
# <a name="iossinglesignonsettings-resource-type"></a>Тип ресурса Иоссинглесигнонсеттингс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры проверки подлинности Kerberos для iOS для единого входа

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаппслист|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список идентификаторов приложений, которым разрешено использовать это имя для входа. Если это поле опущено, имя входа применяется ко всем приложениям на устройстве. Эта коллекция может содержать не более 500 элементов.|
|алловедурлс|Коллекция String|Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа. При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.|
|displayName|String|Отображаемое имя параметров входа, отображаемое на принимающем устройстве.|
|кербероспринЦипалнаме|String|Имя субъекта Kerberos. Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.|
|керберосреалм|String|Имя области Kerberos. С учетом регистра.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```






