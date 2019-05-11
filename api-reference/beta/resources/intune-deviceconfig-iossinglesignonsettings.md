---
title: Тип ресурса Иоссинглесигнонсеттингс
description: Параметры проверки подлинности Kerberos для iOS для единого входа
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75c63454442510b62fe4c7391d4e1a5b86164bca
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946401"
---
# <a name="iossinglesignonsettings-resource-type"></a>Тип ресурса Иоссинглесигнонсеттингс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры проверки подлинности Kerberos для iOS для единого входа

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Алловедаппслист|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список идентификаторов приложений, которым разрешено использовать это имя для входа. Если это поле опущено, имя входа применяется ко всем приложениям на устройстве. Эта коллекция может содержать не более 500 элементов.|
|Алловедурлс|Коллекция строк|Список URL-адресов HTTP, которые должны быть сопоставлены для использования этого имени входа. При использовании iOS 9,0 или более поздних версий можно использовать подстановочные знаки.|
|displayName|Строка|Отображаемое имя параметров входа, отображаемое на принимающем устройстве.|
|КербероспринЦипалнаме|Строка|Имя субъекта Kerberos. Если этот параметр не указан, пользователю предлагается указать один во время установки профиля.|
|Керберосреалм|Строка|Имя области Kerberos. С учетом регистра.|

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




