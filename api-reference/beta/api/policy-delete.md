---
title: Удаление политики
description: Удаление политики.
ms.openlocfilehash: 37ed08e7f53db726a46821c08d68c955afdacc5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082110"
---
# <a name="delete-policy"></a><span data-ttu-id="79735-103">Удаление политики</span><span class="sxs-lookup"><span data-stu-id="79735-103">Delete Policy</span></span>

> <span data-ttu-id="79735-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79735-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79735-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79735-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79735-106">Удаление [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="79735-106">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79735-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79735-107">Permissions</span></span>
<span data-ttu-id="79735-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79735-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79735-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79735-110">Permission type</span></span>      | <span data-ttu-id="79735-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79735-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79735-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79735-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79735-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79735-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79735-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79735-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79735-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79735-115">Not supported.</span></span>    |
|<span data-ttu-id="79735-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79735-116">Application</span></span> | <span data-ttu-id="79735-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79735-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79735-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79735-118">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79735-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79735-119">Request headers</span></span>
| <span data-ttu-id="79735-120">Имя</span><span class="sxs-lookup"><span data-stu-id="79735-120">Name</span></span>       | <span data-ttu-id="79735-121">Тип</span><span class="sxs-lookup"><span data-stu-id="79735-121">Type</span></span> | <span data-ttu-id="79735-122">Описание</span><span class="sxs-lookup"><span data-stu-id="79735-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79735-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79735-123">Authorization</span></span>  | <span data-ttu-id="79735-124">string</span><span class="sxs-lookup"><span data-stu-id="79735-124">string</span></span>  | <span data-ttu-id="79735-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79735-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79735-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79735-127">Request body</span></span>
<span data-ttu-id="79735-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79735-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79735-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="79735-129">Response</span></span>

<span data-ttu-id="79735-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79735-130">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="79735-131">В случае неудачи...</span><span class="sxs-lookup"><span data-stu-id="79735-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="79735-132">Пример</span><span class="sxs-lookup"><span data-stu-id="79735-132">Example</span></span>
<span data-ttu-id="79735-133">В следующем примере удаляется политика.</span><span class="sxs-lookup"><span data-stu-id="79735-133">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="79735-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="79735-134">Request</span></span>
<span data-ttu-id="79735-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79735-135">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="79735-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="79735-136">Response</span></span>
<span data-ttu-id="79735-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="79735-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
