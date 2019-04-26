---
title: Удаление политики
description: Удаление политики.
localization_priority: Normal
ms.openlocfilehash: 6467259fc0cca067deb25bc561ddf18f54760e92
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337462"
---
# <a name="delete-policy"></a><span data-ttu-id="3255d-103">Удаление политики</span><span class="sxs-lookup"><span data-stu-id="3255d-103">Delete Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3255d-104">Удаление [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="3255d-104">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3255d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3255d-105">Permissions</span></span>
<span data-ttu-id="3255d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3255d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3255d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3255d-108">Permission type</span></span>      | <span data-ttu-id="3255d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3255d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3255d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3255d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3255d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3255d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3255d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3255d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3255d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3255d-113">Not supported.</span></span>    |
|<span data-ttu-id="3255d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3255d-114">Application</span></span> | <span data-ttu-id="3255d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3255d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3255d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3255d-116">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3255d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3255d-117">Request headers</span></span>
| <span data-ttu-id="3255d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3255d-118">Name</span></span>       | <span data-ttu-id="3255d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3255d-119">Type</span></span> | <span data-ttu-id="3255d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3255d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3255d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3255d-121">Authorization</span></span>  | <span data-ttu-id="3255d-122">string</span><span class="sxs-lookup"><span data-stu-id="3255d-122">string</span></span>  | <span data-ttu-id="3255d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3255d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3255d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3255d-125">Request body</span></span>
<span data-ttu-id="3255d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3255d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3255d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3255d-127">Response</span></span>

<span data-ttu-id="3255d-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3255d-128">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="3255d-129">В случае неудачного завершения...</span><span class="sxs-lookup"><span data-stu-id="3255d-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="3255d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3255d-130">Example</span></span>
<span data-ttu-id="3255d-131">В следующем примере удаляется политика.</span><span class="sxs-lookup"><span data-stu-id="3255d-131">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="3255d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3255d-132">Request</span></span>
<span data-ttu-id="3255d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3255d-133">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="3255d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3255d-134">Response</span></span>
<span data-ttu-id="3255d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3255d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
