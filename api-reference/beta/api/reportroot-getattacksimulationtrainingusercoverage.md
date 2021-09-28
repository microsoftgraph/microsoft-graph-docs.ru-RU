---
title: 'reportRoot: getAttackSimulationTrainingUserCoverage'
description: Список обучающих покрытий для пользователей клиента в кампаниях моделирования атак и учебных кампаний.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: ddda75fe00fa548ffc2ac7e01492e6a0864a73ec
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979797"
---
# <a name="reportroot-getattacksimulationtrainingusercoverage"></a>reportRoot: getAttackSimulationTrainingUserCoverage
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список [обучающих покрытий](../resources/attacksimulationtrainingusercoverage.md) для каждого пользователя клиента в кампаниях моделирования атак и учебных кампаний.

Эта функция поддерживает `@odata.nextLink` pagination.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All                            |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Reports.Read.All                            |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getAttackSimulationTrainingUserCoverage
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию attackSimulationTrainingUserCoverage](../resources/attacksimulationtrainingusercoverage.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "reportroot_getattacksimulationtrainingusercoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getAttackSimulationTrainingUserCoverage
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attackSimulationTrainingUserCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "userTrainings": [
        {
          "assignedDateTime": "2021-01-01T01:01:01.01Z",
          "completionDateTime": "2021-01-02T01:01:01.01Z",
          "trainingStatus": "Completed",
          "displayName": "Sample Training"
        }
      ],
      "attackSimulationUser": {
        "userId": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      }
    }
  ]
}
```

