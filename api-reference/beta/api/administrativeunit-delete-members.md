---
title: Удаление члена
description: Используйте этот интерфейс API для удаления участника (пользователя или группы) из административного подразделения.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e79dac5b7ae3a20675f6faaf9b209f8117ca2252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941529"
---
# <a name="remove-a-member"></a><span data-ttu-id="2c151-103">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="2c151-103">Remove a member</span></span>

> <span data-ttu-id="2c151-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c151-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c151-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c151-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c151-106">Используйте этот интерфейс API для удаления участника (пользователя или группы) из административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="2c151-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c151-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c151-107">Permissions</span></span>
<span data-ttu-id="2c151-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c151-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2c151-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c151-110">Permission type</span></span>      | <span data-ttu-id="2c151-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c151-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c151-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c151-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c151-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c151-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c151-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c151-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c151-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c151-115">Not supported.</span></span>    |
|<span data-ttu-id="2c151-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c151-116">Application</span></span> | <span data-ttu-id="2c151-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c151-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c151-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c151-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2c151-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c151-119">Request headers</span></span>
| <span data-ttu-id="2c151-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2c151-120">Name</span></span>      |<span data-ttu-id="2c151-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2c151-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c151-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c151-122">Authorization</span></span>  | <span data-ttu-id="2c151-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c151-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c151-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c151-125">Request body</span></span>
<span data-ttu-id="2c151-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c151-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c151-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c151-127">Response</span></span>

<span data-ttu-id="2c151-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2c151-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c151-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2c151-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c151-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c151-131">Request</span></span>
<span data-ttu-id="2c151-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c151-132">Here is an example of the request.</span></span> <span data-ttu-id="2c151-133">В приведенном ниже примере id1 представляет идентификатор для конечного единица и id2 представляет уникальный идентификатор участника пользователя или группы для удаления из targetted единица.</span><span class="sxs-lookup"><span data-stu-id="2c151-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="2c151-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c151-134">Response</span></span>
<span data-ttu-id="2c151-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c151-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
