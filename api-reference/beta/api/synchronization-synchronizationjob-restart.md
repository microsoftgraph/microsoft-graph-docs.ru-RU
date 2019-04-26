---
title: Перезапуск Синчронизатионжоб
description: ПереЗапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге. При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.
localization_priority: Normal
ms.openlocfilehash: 8ef1a4ede6cee7e1ed86e90e329401bcf801e129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330435"
---
# <a name="restart-synchronizationjob"></a>Перезапуск Синчронизатионжоб

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ПереЗапустите задание синхронизации, чтобы принудительно обработать все объекты в каталоге. При необходимости можно очистить существующее состояние синхронизации и предыдущие ошибки.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     |Directory.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |Не поддерживается. |
|Для приложений                            |Не поддерживается.  | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Тип    | Описание|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите объект JSON со следующим параметром.

| Параметр     | Тип      | Описание    |
|:--------------|:----------|:---------------|
|criteria       |[Синчронизатионжобрестарткритериа](../resources/synchronization-synchronizationjobrestartcriteria.md) |Условия переЗапуска|

## <a name="response"></a>Отклик

В случае успеха возвращает `204 No Content` отклик. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
