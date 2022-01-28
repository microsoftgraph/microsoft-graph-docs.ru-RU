---
title: 'teamworkDevice: updateSoftware'
description: Обновление программного обеспечения для Microsoft Teams устройства с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 9e2435dc52b88e836874ceae1b3e62bd09fdaec5
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262687"
---
# <a name="teamworkdevice-updatesoftware"></a>teamworkDevice: updateSoftware
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление программного обеспечения для Microsoft Teams устройства с включенной [поддержкой](../resources/teamworkdevice.md). Этот API запускает долгосрочную операцию.

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamworkDevice.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teamwork/devices/{teamworkDeviceId}/updateSoftware
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|softwareType|teamworkSoftwareType|Тип программного обеспечения для обновления. Допустимые типы: `adminAgent`, `teamsClient``operatingSystem`, , `firmware`, `companyPortal``partnerAgent`.|
|softwareVersion|String|Указывает версию программного обеспечения, доступного для обновления.|



## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `202 Accepted`. В ответе также будет содержаться `Location` заглавный заговор, содержащий расположение ресурса [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) . Вы можете проверить состояние операции обновления программного обеспечения, сделав запрос GET `queued`в это расположение, которое возвращает, является ли операция , `succeeded`или `failed`.

Этот метод также возвращает код `409 Conflict` ответа, если операция уже находится в состоянии очереди.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "teamworkdevice_updatesoftware"
}
-->
``` http
POST https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/updateSoftware
Content-Type: application/json
Content-length: 64

{
  "softwareType": "teamsClient",
  "softwareVersion": "1.0.96.22"
}
```


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Location: /teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations/119eb06d-0c4b-4fb3-a754-33dd0d6b618c
Content-Type: text/plain
Content-Length: 0
```

