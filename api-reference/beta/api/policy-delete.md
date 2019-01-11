---
title: Удаление политики
description: Удаление политики.
localization_priority: Normal
ms.openlocfilehash: 66772865fdff5ebf4b111cae91e60b00707bf6a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875365"
---
# <a name="delete-policy"></a><span data-ttu-id="8ca04-103">Удаление политики</span><span class="sxs-lookup"><span data-stu-id="8ca04-103">Delete Policy</span></span>

> <span data-ttu-id="8ca04-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8ca04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ca04-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ca04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ca04-106">Удаление [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="8ca04-106">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ca04-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ca04-107">Permissions</span></span>
<span data-ttu-id="8ca04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ca04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ca04-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ca04-110">Permission type</span></span>      | <span data-ttu-id="8ca04-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ca04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ca04-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ca04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8ca04-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ca04-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ca04-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ca04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ca04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ca04-115">Not supported.</span></span>    |
|<span data-ttu-id="8ca04-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ca04-116">Application</span></span> | <span data-ttu-id="8ca04-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ca04-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ca04-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ca04-118">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8ca04-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ca04-119">Request headers</span></span>
| <span data-ttu-id="8ca04-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8ca04-120">Name</span></span>       | <span data-ttu-id="8ca04-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8ca04-121">Type</span></span> | <span data-ttu-id="8ca04-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8ca04-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ca04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ca04-123">Authorization</span></span>  | <span data-ttu-id="8ca04-124">string</span><span class="sxs-lookup"><span data-stu-id="8ca04-124">string</span></span>  | <span data-ttu-id="8ca04-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ca04-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ca04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ca04-127">Request body</span></span>
<span data-ttu-id="8ca04-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ca04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ca04-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ca04-129">Response</span></span>

<span data-ttu-id="8ca04-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8ca04-130">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="8ca04-131">В случае неудачи...</span><span class="sxs-lookup"><span data-stu-id="8ca04-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="8ca04-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8ca04-132">Example</span></span>
<span data-ttu-id="8ca04-133">В следующем примере удаляется политика.</span><span class="sxs-lookup"><span data-stu-id="8ca04-133">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="8ca04-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ca04-134">Request</span></span>
<span data-ttu-id="8ca04-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ca04-135">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="8ca04-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ca04-136">Response</span></span>
<span data-ttu-id="8ca04-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8ca04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
