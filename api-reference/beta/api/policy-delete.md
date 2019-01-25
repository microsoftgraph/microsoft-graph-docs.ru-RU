---
title: Удаление политики
description: Удаление политики.
localization_priority: Normal
ms.openlocfilehash: e4e5f5372e2904e1f74bc25224e3d2b1ce7ba154
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520440"
---
# <a name="delete-policy"></a><span data-ttu-id="e4b91-103">Удаление политики</span><span class="sxs-lookup"><span data-stu-id="e4b91-103">Delete Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4b91-104">Удаление [политики](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="e4b91-104">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4b91-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b91-105">Permissions</span></span>
<span data-ttu-id="e4b91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4b91-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b91-108">Permission type</span></span>      | <span data-ttu-id="e4b91-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4b91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4b91-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4b91-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4b91-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4b91-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4b91-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4b91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4b91-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b91-113">Not supported.</span></span>    |
|<span data-ttu-id="e4b91-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4b91-114">Application</span></span> | <span data-ttu-id="e4b91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b91-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4b91-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4b91-116">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e4b91-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4b91-117">Request headers</span></span>
| <span data-ttu-id="e4b91-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e4b91-118">Name</span></span>       | <span data-ttu-id="e4b91-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e4b91-119">Type</span></span> | <span data-ttu-id="e4b91-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b91-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e4b91-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4b91-121">Authorization</span></span>  | <span data-ttu-id="e4b91-122">string</span><span class="sxs-lookup"><span data-stu-id="e4b91-122">string</span></span>  | <span data-ttu-id="e4b91-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4b91-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4b91-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4b91-125">Request body</span></span>
<span data-ttu-id="e4b91-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4b91-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4b91-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4b91-127">Response</span></span>

<span data-ttu-id="e4b91-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4b91-128">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="e4b91-129">В случае неудачи...</span><span class="sxs-lookup"><span data-stu-id="e4b91-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="e4b91-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e4b91-130">Example</span></span>
<span data-ttu-id="e4b91-131">В следующем примере удаляется политика.</span><span class="sxs-lookup"><span data-stu-id="e4b91-131">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="e4b91-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4b91-132">Request</span></span>
<span data-ttu-id="e4b91-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4b91-133">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="e4b91-134">Отклик
</span><span class="sxs-lookup"><span data-stu-id="e4b91-134">Response</span></span>
<span data-ttu-id="e4b91-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e4b91-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
