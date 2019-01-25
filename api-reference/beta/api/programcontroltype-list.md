---
title: Список programControlTypes
description: В Azure AD доступа к функции проверки, список всех объектов programControlType.
localization_priority: Normal
ms.openlocfilehash: 00983cadf4bd1e0cf136c594f06ac3ee6fbb1de5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515694"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="f36de-103">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="f36de-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f36de-104">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [programControlType](../resources/programcontroltype.md) .</span><span class="sxs-lookup"><span data-stu-id="f36de-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f36de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f36de-105">Permissions</span></span>
<span data-ttu-id="f36de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f36de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f36de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f36de-108">Permission type</span></span>                        | <span data-ttu-id="f36de-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f36de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f36de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f36de-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f36de-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f36de-111"></span></span>  <span data-ttu-id="f36de-112">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать программы.</span><span class="sxs-lookup"><span data-stu-id="f36de-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="f36de-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f36de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f36de-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f36de-114">Not supported.</span></span> |
|<span data-ttu-id="f36de-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f36de-115">Application</span></span>                            | <span data-ttu-id="f36de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f36de-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f36de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f36de-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="f36de-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f36de-118">Request headers</span></span>
| <span data-ttu-id="f36de-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f36de-119">Name</span></span>         | <span data-ttu-id="f36de-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f36de-120">Type</span></span>        | <span data-ttu-id="f36de-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f36de-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f36de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f36de-122">Authorization</span></span> | <span data-ttu-id="f36de-123">string</span><span class="sxs-lookup"><span data-stu-id="f36de-123">string</span></span> | <span data-ttu-id="f36de-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="f36de-124">Bearer \{token\}.</span></span> <span data-ttu-id="f36de-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f36de-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f36de-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f36de-126">Request body</span></span>
<span data-ttu-id="f36de-127">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="f36de-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f36de-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f36de-128">Response</span></span>
<span data-ttu-id="f36de-129">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [programControlType](../resources/programcontroltype.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f36de-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f36de-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f36de-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f36de-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f36de-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="f36de-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f36de-132">Response</span></span>
><span data-ttu-id="f36de-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f36de-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="f36de-135">См. также</span><span class="sxs-lookup"><span data-stu-id="f36de-135">See also</span></span>

| <span data-ttu-id="f36de-136">Метод</span><span class="sxs-lookup"><span data-stu-id="f36de-136">Method</span></span>           | <span data-ttu-id="f36de-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f36de-137">Return Type</span></span>    |<span data-ttu-id="f36de-138">Описание</span><span class="sxs-lookup"><span data-stu-id="f36de-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f36de-139">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="f36de-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="f36de-140">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f36de-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="f36de-141">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="f36de-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
