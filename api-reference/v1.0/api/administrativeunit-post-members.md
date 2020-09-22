---
title: Добавление участника
description: Используйте этот API, чтобы добавить члена (пользователя или группы) в административную единицу.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 618ece1f8123044c0f5a8b73702876bd77266aef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020322"
---
# <a name="add-a-member"></a>Добавление участника

Пространство имен: microsoft.graph

Используйте этот API, чтобы добавить члена (пользователя или группы) в административную единицу.

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AdministrativeUnit.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите `id` [пользователя](../resources/user.md),  [группу](../resources/group.md) или [directoryObject](../resources/directoryobject.md) , которого требуется добавить.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/v1.0/groups/{id}"
}

```
В тексте запроса укажите `id` объект [пользователя](../resources/user.md) или [группы](../resources/group.md) , который вы хотите добавить.

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
 
```http
HTTP/1.1 204 No Content
```
