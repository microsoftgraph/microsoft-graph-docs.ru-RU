---
title: Список programControls программы
description: В Azure AD access дается обзор компонента, список всех programControl объектов, связанные с определенной программе.
localization_priority: Normal
ms.openlocfilehash: 9134e9aa322446553da2e0c644a6fc8b43b0b54d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508267"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="7a42d-103">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="7a42d-103">List programControls of a program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a42d-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD перечислены все [programControl](../resources/programcontrol.md) объекты, связанные с определенной программе.</span><span class="sxs-lookup"><span data-stu-id="7a42d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a42d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a42d-105">Permissions</span></span>
<span data-ttu-id="7a42d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a42d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a42d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a42d-108">Permission type</span></span>                        | <span data-ttu-id="7a42d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a42d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a42d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a42d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a42d-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="7a42d-111"></span></span>  <span data-ttu-id="7a42d-112">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать программы.</span><span class="sxs-lookup"><span data-stu-id="7a42d-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="7a42d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a42d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a42d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a42d-114">Not supported.</span></span> |
|<span data-ttu-id="7a42d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a42d-115">Application</span></span>                            | <span data-ttu-id="7a42d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a42d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a42d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a42d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="7a42d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a42d-118">Request headers</span></span>
| <span data-ttu-id="7a42d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7a42d-119">Name</span></span>         | <span data-ttu-id="7a42d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7a42d-120">Type</span></span>        | <span data-ttu-id="7a42d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7a42d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7a42d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a42d-122">Authorization</span></span> | <span data-ttu-id="7a42d-123">string</span><span class="sxs-lookup"><span data-stu-id="7a42d-123">string</span></span> | <span data-ttu-id="7a42d-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="7a42d-124">Bearer \{token\}.</span></span> <span data-ttu-id="7a42d-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a42d-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a42d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a42d-126">Request body</span></span>
<span data-ttu-id="7a42d-127">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="7a42d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="7a42d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a42d-128">Response</span></span>
<span data-ttu-id="7a42d-129">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [programControl](../resources/programcontrol.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a42d-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a42d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7a42d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a42d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a42d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs('673a7379-9c38-4f01-bd9d-4fda7260b807')/controls
```

##### <a name="response"></a><span data-ttu-id="7a42d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a42d-132">Response</span></span>
><span data-ttu-id="7a42d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a42d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-listcontrols.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
