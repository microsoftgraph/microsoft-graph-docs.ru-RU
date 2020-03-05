---
title: Удаление политики
description: Удаление политики.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d86f4011df727ec31e2c054e0fa2ea10736ca9e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455533"
---
# <a name="delete-policy"></a><span data-ttu-id="629aa-103">Удаление политики</span><span class="sxs-lookup"><span data-stu-id="629aa-103">Delete Policy</span></span>

<span data-ttu-id="629aa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="629aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="629aa-105">Удаление [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="629aa-105">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="629aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="629aa-106">Permissions</span></span>
<span data-ttu-id="629aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="629aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="629aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="629aa-109">Permission type</span></span>      | <span data-ttu-id="629aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="629aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="629aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="629aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="629aa-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="629aa-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="629aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="629aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="629aa-114">Not supported.</span></span>    |
|<span data-ttu-id="629aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="629aa-115">Application</span></span> | <span data-ttu-id="629aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="629aa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="629aa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="629aa-117">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="629aa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="629aa-118">Request headers</span></span>
| <span data-ttu-id="629aa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="629aa-119">Name</span></span>       | <span data-ttu-id="629aa-120">Тип</span><span class="sxs-lookup"><span data-stu-id="629aa-120">Type</span></span> | <span data-ttu-id="629aa-121">Описание</span><span class="sxs-lookup"><span data-stu-id="629aa-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="629aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="629aa-122">Authorization</span></span>  | <span data-ttu-id="629aa-123">string</span><span class="sxs-lookup"><span data-stu-id="629aa-123">string</span></span>  | <span data-ttu-id="629aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="629aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="629aa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="629aa-126">Request body</span></span>
<span data-ttu-id="629aa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="629aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="629aa-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="629aa-128">Response</span></span>

<span data-ttu-id="629aa-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="629aa-129">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="629aa-130">В случае неудачного завершения...</span><span class="sxs-lookup"><span data-stu-id="629aa-130">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="629aa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="629aa-131">Example</span></span>
<span data-ttu-id="629aa-132">В следующем примере удаляется политика.</span><span class="sxs-lookup"><span data-stu-id="629aa-132">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="629aa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="629aa-133">Request</span></span>
<span data-ttu-id="629aa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="629aa-134">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="629aa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="629aa-135">Response</span></span>
<span data-ttu-id="629aa-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="629aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
