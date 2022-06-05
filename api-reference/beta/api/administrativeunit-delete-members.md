---
title: Удаление участника
description: Используйте этот API, чтобы удалить участника (пользователя, группу или устройство) из административной единицы.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 199e0ba76a61b8279dcd79acb59ef14d9001a35d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898170"
---
# <a name="remove-a-member"></a>Удаление участника

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте этот API, чтобы удалить участника (пользователя, группу или устройство) из административной единицы.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | AdministrativeUnit.ReadWrite.All   |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Application | AdministrativeUnit.ReadWrite.All |

Чтобы удалить участника из административной единицы, вызывающему субъекту должна быть назначена одна из следующих ролей [Azure AD](/azure/active-directory/roles/permissions-reference):

* Администратор привилегированных ролей
* Глобальный администратор

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса. `{id1}` `{id2}` В приведенном ниже примере представляет идентификатор целевой административной единицы и уникальный идентификатор пользователя, группы или устройства, удаляемого из целевой административной единицы. 

```msgraph-interactive
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
 
```http
HTTP/1.1 204 No Content
```


