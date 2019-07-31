---
title: Получение члена
description: Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81a1165148dbaa81740cdc4d7b9dbf65f7d8cd4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945860"
---
# <a name="get-a-member"></a>Получение члена

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [User](../resources/user.md) или [Group](../resources/group.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a>Отклик
Ниже приведен пример респоне. Примечание. Представленный здесь объект ответа может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```
