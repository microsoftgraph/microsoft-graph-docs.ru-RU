---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20c6cabbd5f18349058c68136052c8d56894dccc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728565"
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
|алловедурлс|Коллекция строк|Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа. При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.|
|displayName|Строка|Отображаемое имя параметров входа, отображаемое на принимающем устройстве.|
|кербероспринЦипалнаме|Строка|Имя субъекта Kerberos. Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.|
|керберосреалм|Строка|Имя области Kerberos. С учетом регистра.|

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





