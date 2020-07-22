---
title: 'directoryObject: Жетаваилабликстенсионпропертиес'
description: Получение всех или отфильтрованных списков свойств расширения каталога, зарегистрированных в каталоге.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3276b114f3fa6370a4cc8d03b8b6607148bf3c7f
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225009"
---
# <a name="directoryobject-getavailableextensionproperties"></a>directoryObject: Жетаваилабликстенсионпропертиес
Пространство имен: microsoft.graph

Возвращает все или отфильтрованный список свойств расширения каталога, зарегистрированных в каталоге. Следующие объекты поддерживают свойства расширения: **User**, **Group**, **Organization**, **Device**, **Application**и **servicePrincipal**.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| Directory.Read.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Directory.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directoryObjects/getAvailableExtensionProperties
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|иссинцедфромонпремисес|Boolean|`true`чтобы указать, что необходимо вернуть только свойства расширения, синхронизированные из локального каталога; `false`чтобы указать, что необходимо вернуть только свойства расширения, которые не синхронизируются из локального каталога. Если параметр не задан, возвращаются все свойства расширения (синхронизированные и несинхронизированные).|


## <a name="response"></a>Отклик

При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "directoryobject_getavailableextensionproperties"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/getAvailableExtensionProperties

Content-Type: application/json
Content-length: 43

{
  "isSyncedFromOnPremises": "Boolean"
}
```

### <a name="response"></a>Отклик
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.extensionProperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.extensionProperty",
      "id": "d6a8bfec-893d-46e4-88fd-7db5fcc0fa62",
      "deletedDateTime": null,
      "appDisplayName": "SampleApp",
      "name": "extension_4d405aa8baa04fb494d3e0571fd9fd71_skypeId",
      "dataType": "String",
      "isSyncedFromOnPremises": false,
      "targetObjects": [
        "User"
      ]
    }
  ]
}
```

