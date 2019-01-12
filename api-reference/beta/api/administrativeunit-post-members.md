---
title: Добавить участника
description: Используйте этот интерфейс API для добавления элемента (пользователя или группы) для административного подразделения.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f64ca4c00265903fa1b4ebc467f2d70274628078
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946828"
---
# <a name="add-a-member"></a>Добавить участника

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используйте этот интерфейс API для добавления элемента (пользователя или группы) для административного подразделения.

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON [пользователя](../resources/user.md), [группы](../resources/group.md) или [directoryObject](../resources/directoryobject.md) для добавления.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
В тексте запроса укажите представление JSON `id` объекта [пользователя](../resources/user.md) или [группы](../resources/group.md) , необходимо добавить.

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
 
```http
HTTP/1.1 204 No Content
```
