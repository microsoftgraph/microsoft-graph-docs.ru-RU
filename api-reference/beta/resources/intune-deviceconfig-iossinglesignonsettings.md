---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5f35240243b94a2abdc817823b70d53a64b43dca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529855"
---
# <a name="iossinglesignonsettings-resource-type"></a>Тип ресурса Иоссинглесигнонсеттингс

Пространство имен: Microsoft. Graph

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

## <a name="relationships"></a>Связи
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



