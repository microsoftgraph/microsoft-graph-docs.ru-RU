---
title: Добавить участника
description: Используйте этот интерфейс API для добавления элемента (пользователя или группы) для административного подразделения.
author: lleonard-msft
ms.openlocfilehash: be47dbf06c5f59c0a4aaaea4f8c8b4aa8c3ce902
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339230"
---
# <a name="add-a-member"></a><span data-ttu-id="11e6a-103">Добавить участника</span><span class="sxs-lookup"><span data-stu-id="11e6a-103">Add a member</span></span>

> <span data-ttu-id="11e6a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11e6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11e6a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11e6a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11e6a-106">Используйте этот интерфейс API для добавления элемента (пользователя или группы) для административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="11e6a-106">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="11e6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11e6a-107">Permissions</span></span>
<span data-ttu-id="11e6a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="11e6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11e6a-110">Permission type</span></span>      | <span data-ttu-id="11e6a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11e6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11e6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11e6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="11e6a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11e6a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11e6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11e6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11e6a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11e6a-115">Not supported.</span></span>    |
|<span data-ttu-id="11e6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11e6a-116">Application</span></span> | <span data-ttu-id="11e6a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11e6a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11e6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11e6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="11e6a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11e6a-119">Request headers</span></span>
| <span data-ttu-id="11e6a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="11e6a-120">Name</span></span>      |<span data-ttu-id="11e6a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="11e6a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11e6a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11e6a-122">Authorization</span></span>  | <span data-ttu-id="11e6a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11e6a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11e6a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11e6a-125">Request body</span></span>
<span data-ttu-id="11e6a-126">В тексте запроса укажите представление JSON [пользователя](../resources/user.md), [группы](../resources/group.md) или [directoryObject](../resources/directoryobject.md) для добавления.</span><span class="sxs-lookup"><span data-stu-id="11e6a-126">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="11e6a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="11e6a-127">Response</span></span>

<span data-ttu-id="11e6a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="11e6a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11e6a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="11e6a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11e6a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="11e6a-131">Request</span></span>
<span data-ttu-id="11e6a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11e6a-132">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="11e6a-133">В тексте запроса укажите представление JSON `id` объекта [пользователя](../resources/user.md) или [группы](../resources/group.md) , необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="11e6a-133">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="11e6a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="11e6a-134">Response</span></span>
<span data-ttu-id="11e6a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11e6a-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
