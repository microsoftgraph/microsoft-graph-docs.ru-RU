---
title: Удаление члена
description: Используйте этот интерфейс API для удаления участника (пользователя или группы) из административного подразделения.
author: lleonard-msft
ms.openlocfilehash: 0b7b03042982b1eb50d9dfd7382186f0b3d28469
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353419"
---
# <a name="remove-a-member"></a><span data-ttu-id="a9491-103">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="a9491-103">Remove a member</span></span>

> <span data-ttu-id="a9491-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9491-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9491-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9491-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9491-106">Используйте этот интерфейс API для удаления участника (пользователя или группы) из административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="a9491-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9491-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9491-107">Permissions</span></span>
<span data-ttu-id="a9491-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9491-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a9491-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9491-110">Permission type</span></span>      | <span data-ttu-id="a9491-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9491-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9491-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9491-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a9491-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9491-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9491-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9491-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9491-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9491-115">Not supported.</span></span>    |
|<span data-ttu-id="a9491-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9491-116">Application</span></span> | <span data-ttu-id="a9491-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9491-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9491-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9491-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a9491-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9491-119">Request headers</span></span>
| <span data-ttu-id="a9491-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a9491-120">Name</span></span>      |<span data-ttu-id="a9491-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a9491-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9491-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9491-122">Authorization</span></span>  | <span data-ttu-id="a9491-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9491-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9491-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9491-125">Request body</span></span>
<span data-ttu-id="a9491-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9491-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9491-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9491-127">Response</span></span>

<span data-ttu-id="a9491-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a9491-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9491-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a9491-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9491-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9491-131">Request</span></span>
<span data-ttu-id="a9491-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9491-132">Here is an example of the request.</span></span> <span data-ttu-id="a9491-133">В приведенном ниже примере id1 представляет идентификатор для конечного единица и id2 представляет уникальный идентификатор участника пользователя или группы для удаления из targetted единица.</span><span class="sxs-lookup"><span data-stu-id="a9491-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="a9491-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9491-134">Response</span></span>
<span data-ttu-id="a9491-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a9491-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
