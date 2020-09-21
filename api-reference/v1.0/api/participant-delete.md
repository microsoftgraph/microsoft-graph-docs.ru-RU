---
title: Удаление участника
description: Удаление определенного участника в вызове.
manager: zhengni
author: jackry6350
ms.author: yoren
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8c08821f723152adb82cde0255d21ea3d8718a8e
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137160"
---
# <a name="delete-participant"></a>Удаление участника

Удаление определенного участника в вызове. В некоторых ситуациях приложение может удалить участника из активного вызова. Это действие можно выполнить как до, так и после того, как участник ответит на звонок. После удаления активного вызывающего абонента он сразу же удаляется из вызова без уведомления о допуске или после удаления.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | Нет                                        |

Настройка собраний для приложения на уровне клиента необходима для того, чтобы приложение мог вызывать этот API. Администратор клиента должен вызвать следующий командлет в удаленной оболочке PowerShell клиента, чтобы предоставить приложению разрешение на вызов этого API. Дополнительные сведения см. в статье [Set – ксаппликатионмитингконфигуратион](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}/participants/{id}
```

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже показан пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/{id}
```

##### <a name="response"></a>Отклик

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
