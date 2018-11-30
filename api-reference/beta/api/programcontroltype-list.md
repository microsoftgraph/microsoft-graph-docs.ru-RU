---
title: Список programControlTypes
description: В Azure AD доступа к функции проверки, список всех объектов programControlType.
ms.openlocfilehash: 9e3b8efccd8d8be96ef1295dfba1a5c2e329c756
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082779"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="abdbd-103">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="abdbd-103">List programControlTypes</span></span>

> <span data-ttu-id="abdbd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abdbd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abdbd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdbd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abdbd-106">В функции [доступа дается обзор](../resources/accessreviews-root.md) Azure AD список всех объектов [programControlType](../resources/programcontroltype.md) .</span><span class="sxs-lookup"><span data-stu-id="abdbd-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="abdbd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abdbd-107">Permissions</span></span>
<span data-ttu-id="abdbd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abdbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abdbd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abdbd-110">Permission type</span></span>                        | <span data-ttu-id="abdbd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abdbd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="abdbd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abdbd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="abdbd-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="abdbd-113"></span></span>  <span data-ttu-id="abdbd-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать программы.</span><span class="sxs-lookup"><span data-stu-id="abdbd-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="abdbd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abdbd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abdbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdbd-116">Not supported.</span></span> |
|<span data-ttu-id="abdbd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abdbd-117">Application</span></span>                            | <span data-ttu-id="abdbd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdbd-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abdbd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abdbd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="abdbd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abdbd-120">Request headers</span></span>
| <span data-ttu-id="abdbd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="abdbd-121">Name</span></span>         | <span data-ttu-id="abdbd-122">Тип</span><span class="sxs-lookup"><span data-stu-id="abdbd-122">Type</span></span>        | <span data-ttu-id="abdbd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="abdbd-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="abdbd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="abdbd-124">Authorization</span></span> | <span data-ttu-id="abdbd-125">string</span><span class="sxs-lookup"><span data-stu-id="abdbd-125">string</span></span> | <span data-ttu-id="abdbd-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="abdbd-126">Bearer \{token\}.</span></span> <span data-ttu-id="abdbd-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="abdbd-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abdbd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abdbd-128">Request body</span></span>
<span data-ttu-id="abdbd-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="abdbd-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="abdbd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="abdbd-130">Response</span></span>
<span data-ttu-id="abdbd-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [programControlType](../resources/programcontroltype.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="abdbd-131">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abdbd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="abdbd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abdbd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="abdbd-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="abdbd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="abdbd-134">Response</span></span>
><span data-ttu-id="abdbd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abdbd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="abdbd-137">См. также</span><span class="sxs-lookup"><span data-stu-id="abdbd-137">See also</span></span>

| <span data-ttu-id="abdbd-138">Метод</span><span class="sxs-lookup"><span data-stu-id="abdbd-138">Method</span></span>           | <span data-ttu-id="abdbd-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="abdbd-139">Return Type</span></span>    |<span data-ttu-id="abdbd-140">Описание</span><span class="sxs-lookup"><span data-stu-id="abdbd-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="abdbd-141">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="abdbd-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="abdbd-142">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="abdbd-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="abdbd-143">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="abdbd-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
