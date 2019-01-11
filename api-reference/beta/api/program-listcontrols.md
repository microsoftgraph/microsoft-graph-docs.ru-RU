---
title: Список programControls программы
description: В Azure AD access дается обзор компонента, список всех programControl объектов, связанные с определенной программе.
localization_priority: Normal
ms.openlocfilehash: 8895634b098474cdbeab695cbe730a1e2fd02e2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809339"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="d5a8c-103">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="d5a8c-103">List programControls of a program</span></span>

> <span data-ttu-id="d5a8c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5a8c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5a8c-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD перечислены все [programControl](../resources/programcontrol.md) объекты, связанные с определенной программе.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5a8c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a8c-107">Permissions</span></span>
<span data-ttu-id="d5a8c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5a8c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a8c-110">Permission type</span></span>                        | <span data-ttu-id="d5a8c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5a8c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5a8c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5a8c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5a8c-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-113"></span></span>  <span data-ttu-id="d5a8c-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать программы.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="d5a8c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5a8c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5a8c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-116">Not supported.</span></span> |
|<span data-ttu-id="d5a8c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5a8c-117">Application</span></span>                            | <span data-ttu-id="d5a8c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5a8c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5a8c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="d5a8c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5a8c-120">Request headers</span></span>
| <span data-ttu-id="d5a8c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d5a8c-121">Name</span></span>         | <span data-ttu-id="d5a8c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d5a8c-122">Type</span></span>        | <span data-ttu-id="d5a8c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d5a8c-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d5a8c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5a8c-124">Authorization</span></span> | <span data-ttu-id="d5a8c-125">string</span><span class="sxs-lookup"><span data-stu-id="d5a8c-125">string</span></span> | <span data-ttu-id="d5a8c-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-126">Bearer \{token\}.</span></span> <span data-ttu-id="d5a8c-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5a8c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5a8c-128">Request body</span></span>
<span data-ttu-id="d5a8c-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d5a8c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5a8c-130">Response</span></span>
<span data-ttu-id="d5a8c-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [programControl](../resources/programcontrol.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5a8c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d5a8c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5a8c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a8c-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs('673a7379-9c38-4f01-bd9d-4fda7260b807')/controls
```

##### <a name="response"></a><span data-ttu-id="d5a8c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a8c-134">Response</span></span>
><span data-ttu-id="d5a8c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5a8c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


<!-- {
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
