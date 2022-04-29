---
title: 'cloudPC: getCloudPcLaunchInfo'
description: Получение сведений о запуске облачного компьютера для вошедвшего пользователя.
author: andrewku0409
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 0a83e56df0b4b7de3dc362134aac3981d14d4f91
ms.sourcegitcommit: 4ef29d4a2cfa1ccc4a3da649e683377b17b90108
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65126358"
---
# <a name="cloudpc-getcloudpclaunchinfo"></a>cloudPC: getCloudPcLaunchInfo
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите [cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md) для пользователя, выполнившего вход.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/cloudPCs/{cloudPCId}/getCloudPcLaunchInfo
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения эта функция возвращает код `200 OK` отклика и объект [cloudPcLaunchInfo](../resources/cloudpclaunchinfo.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "cloudpcthis.getcloudpclaunchinfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/cloudPCs/{cloudPCId}/getCloudPcLaunchInfo
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcLaunchInfo"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.cloudPcLaunchInfo",
  "cloudPcId": "a20d556d-85f7-88cc-bb9c-08d9902bb7bb",
  "cloudPcLaunchUrl": "https://rdweb-r0.wvdselfhost.microsoft.com/api/arm/weblaunch/tenants/662009bc-7732-4f6f-8726-25883518b33e/resources/662009bc-7732-4f6f-8726-25883518b33e"
}
```

