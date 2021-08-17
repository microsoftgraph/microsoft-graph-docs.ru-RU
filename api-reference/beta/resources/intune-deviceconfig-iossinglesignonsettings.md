---
title: тип ресурса iosSingleSignOnSettings
description: Параметры проверки подлинности iOS Kerberos для одного входного знака
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 724b6d0deb2fff796c5f7d43d961a014eadc84c2659e47392def0e803c172b5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145399"
---
# <a name="iossinglesignonsettings-resource-type"></a>тип ресурса iosSingleSignOnSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры проверки подлинности iOS Kerberos для одного входного знака

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAppsList|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Список идентификаторов приложений, которые разрешены для использования этого входа. Если это поле опущено, вход применяется ко всем приложениям на устройстве. Эта коллекция может содержать не более 500 элементов.|
|allowedUrls|Коллекция String|Список URL-адресов HTTP, которые необходимо соединять для использования этого входа. С помощью iOS 9.0 или более поздней системы можно использовать символы под диктовки.|
|displayName|Строка|Отображение имени параметров входа, показанных на приемном устройстве.|
|kerberosPrincipalName|Строка|Основное имя Kerberos. Если не предоставлено, пользователю будет предложено одно во время установки профиля.|
|kerberosRealm|String|Имя области Kerberos. Деликатный.|

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




