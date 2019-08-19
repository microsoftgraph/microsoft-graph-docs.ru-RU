---
title: Список Акцессревиевс
description: Получение объектов Акцессревиев для Бусинессфловтемплате.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46c9abdbc0a1d5dca4c4e61d423b23ed31691384
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462704"
---
# <a name="list-accessreviews"></a><span data-ttu-id="840f5-103">Список Акцессревиевс</span><span class="sxs-lookup"><span data-stu-id="840f5-103">List accessReviews</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="840f5-104">Получение объектов [акцессревиев](../resources/accessreview.md) для определенного [бусинессфловтемплате](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="840f5-104">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="840f5-105">Список из нуля или более объектов **акцессревиев** возвращается для каждой одноразовой и повторяющейся проверки доступа, созданной с помощью этого шаблона бизнес-процесса.</span><span class="sxs-lookup"><span data-stu-id="840f5-105">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>

>[!NOTE]
> <span data-ttu-id="840f5-106">Если какой-либо из проверок доступа, соответствующих фильтру, является повторяющейся проверкой доступа, возвращается один объект **акцессревиев** для представления каждого повторяющегося ряда в целом.</span><span class="sxs-lookup"><span data-stu-id="840f5-106">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole.</span></span> <span data-ttu-id="840f5-107">Например, если имеется ежемесячная проверка доступа участников группы "гость", то есть Ежеквартальная проверка доступа участников группы "гость" для группы "б" и одноразовый доступ к просмотру гостевых участников группы C и вызывающим запросом на рецензию доступа с бизнес-процессом шаблон рецензирования участников группы, будут возвращены три объекта.</span><span class="sxs-lookup"><span data-stu-id="840f5-107">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned.</span></span> <span data-ttu-id="840f5-108">Чтобы получить экземпляры повторяющейся проверки доступа или экземпляра проверки доступа, запланированный на определенный месяц или квартал, вызывающий может впоследствии перемещаться по связи **экземпляра** объекта повторяющегося объекта **акцессревиев** .</span><span class="sxs-lookup"><span data-stu-id="840f5-108">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="840f5-109">Связь **экземпляра** связывается с объектами **акцессревиев** для текущего или прошлых экземпляров проверки поповторяющегося доступа.</span><span class="sxs-lookup"><span data-stu-id="840f5-109">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="840f5-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="840f5-110">Permissions</span></span>
<span data-ttu-id="840f5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="840f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="840f5-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="840f5-113">Permission type</span></span>                        | <span data-ttu-id="840f5-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="840f5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="840f5-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="840f5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="840f5-116">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="840f5-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="840f5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="840f5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="840f5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="840f5-118">Not supported.</span></span> |
|<span data-ttu-id="840f5-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="840f5-119">Application</span></span>                            | <span data-ttu-id="840f5-120">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="840f5-120">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="840f5-121">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="840f5-121">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="840f5-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="840f5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}
```
## <a name="request-headers"></a><span data-ttu-id="840f5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="840f5-123">Request headers</span></span>
| <span data-ttu-id="840f5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="840f5-124">Name</span></span>         | <span data-ttu-id="840f5-125">Тип</span><span class="sxs-lookup"><span data-stu-id="840f5-125">Type</span></span>        | <span data-ttu-id="840f5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="840f5-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="840f5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="840f5-127">Authorization</span></span> | <span data-ttu-id="840f5-128">string</span><span class="sxs-lookup"><span data-stu-id="840f5-128">string</span></span> | <span data-ttu-id="840f5-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="840f5-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="840f5-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="840f5-131">Request body</span></span>
<span data-ttu-id="840f5-132">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="840f5-132">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="840f5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="840f5-133">Response</span></span>
<span data-ttu-id="840f5-134">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="840f5-134">If successful, this method returns a `200, OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="840f5-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="840f5-135">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="840f5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="840f5-136">Request</span></span>
<span data-ttu-id="840f5-137">В приведенном ниже примере показан запрос на получение всех одноразовых и повторяющихся проверок доступа для шаблона рабочего процесса "6E4F3D20-C5C3-407F-9695-8460952BCC68".</span><span class="sxs-lookup"><span data-stu-id="840f5-137">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6E4F3D20-C5C3-407F-9695-8460952BCC68'.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="840f5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="840f5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6E4F3D20-C5C3-407F-9695-8460952BCC68'
```


---


##### <a name="response"></a><span data-ttu-id="840f5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="840f5-139">Response</span></span>
><span data-ttu-id="840f5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="840f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="840f5-142">См. также</span><span class="sxs-lookup"><span data-stu-id="840f5-142">See also</span></span>

- [<span data-ttu-id="840f5-143">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="840f5-143">Get accessReview</span></span>](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
