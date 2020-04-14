---
title: Удаление политики
description: Удаление политики.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: c24a20133d79e32d0a2e5559fbc2309b5863aa9b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450888"
---
# <a name="delete-policy"></a><span data-ttu-id="d4c78-103">Удаление политики</span><span class="sxs-lookup"><span data-stu-id="d4c78-103">Delete Policy</span></span>

<span data-ttu-id="d4c78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4c78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4c78-105">Удаление [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="d4c78-105">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4c78-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c78-106">Permissions</span></span>
<span data-ttu-id="d4c78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c78-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c78-109">Permission type</span></span>      | <span data-ttu-id="d4c78-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4c78-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4c78-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4c78-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4c78-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4c78-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4c78-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4c78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4c78-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c78-114">Not supported.</span></span>    |
|<span data-ttu-id="d4c78-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4c78-115">Application</span></span> | <span data-ttu-id="d4c78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c78-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4c78-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4c78-117">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d4c78-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4c78-118">Request headers</span></span>
| <span data-ttu-id="d4c78-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d4c78-119">Name</span></span>       | <span data-ttu-id="d4c78-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d4c78-120">Type</span></span> | <span data-ttu-id="d4c78-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d4c78-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d4c78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4c78-122">Authorization</span></span>  | <span data-ttu-id="d4c78-123">string</span><span class="sxs-lookup"><span data-stu-id="d4c78-123">string</span></span>  | <span data-ttu-id="d4c78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4c78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4c78-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4c78-126">Request body</span></span>
<span data-ttu-id="d4c78-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4c78-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4c78-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4c78-128">Response</span></span>

<span data-ttu-id="d4c78-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d4c78-129">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="d4c78-130">В случае неудачного завершения...</span><span class="sxs-lookup"><span data-stu-id="d4c78-130">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="d4c78-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d4c78-131">Example</span></span>
<span data-ttu-id="d4c78-132">В следующем примере удаляется политика.</span><span class="sxs-lookup"><span data-stu-id="d4c78-132">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="d4c78-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4c78-133">Request</span></span>
<span data-ttu-id="d4c78-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4c78-134">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="d4c78-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4c78-135">Response</span></span>
<span data-ttu-id="d4c78-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4c78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
