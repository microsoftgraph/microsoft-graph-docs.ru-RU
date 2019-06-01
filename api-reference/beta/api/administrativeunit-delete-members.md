---
title: Удаление участника
description: Используйте этот API для удаления члена (пользователя или группы) из административной единицы.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 21bb1fc226f9c16883de32773592ca4bd52a4758
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655413"
---
# <a name="remove-a-member"></a><span data-ttu-id="ac359-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="ac359-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac359-104">Используйте этот API для удаления члена (пользователя или группы) из административной единицы.</span><span class="sxs-lookup"><span data-stu-id="ac359-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac359-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac359-105">Permissions</span></span>
<span data-ttu-id="ac359-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ac359-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac359-108">Permission type</span></span>      | <span data-ttu-id="ac359-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac359-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac359-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac359-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac359-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac359-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac359-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac359-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac359-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac359-113">Not supported.</span></span>    |
|<span data-ttu-id="ac359-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac359-114">Application</span></span> | <span data-ttu-id="ac359-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac359-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac359-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac359-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ac359-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac359-117">Request headers</span></span>
| <span data-ttu-id="ac359-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ac359-118">Name</span></span>      |<span data-ttu-id="ac359-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ac359-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac359-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac359-120">Authorization</span></span>  | <span data-ttu-id="ac359-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac359-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac359-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac359-123">Request body</span></span>
<span data-ttu-id="ac359-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac359-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac359-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac359-125">Response</span></span>

<span data-ttu-id="ac359-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ac359-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac359-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ac359-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac359-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac359-129">Request</span></span>
<span data-ttu-id="ac359-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac359-130">Here is an example of the request.</span></span> <span data-ttu-id="ac359-131">В приведенном ниже примере id1 представляет идентификатор целевого административного подразделения, а id2 представляет уникальный идентификатор удаляемого пользователя или группы из административного модуля адресного.</span><span class="sxs-lookup"><span data-stu-id="ac359-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="ac359-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac359-132">Response</span></span>
<span data-ttu-id="ac359-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac359-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
