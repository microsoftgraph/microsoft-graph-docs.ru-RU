---
author: swapnil1993
title: Обновление contentType
description: Обновление типа контента
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 86900c12750fdd149025c230b3386d5e5f0eeddd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447212"
---
# <a name="update-contenttype"></a><span data-ttu-id="455a3-103">Обновление contentType</span><span class="sxs-lookup"><span data-stu-id="455a3-103">Update contentType</span></span>
<span data-ttu-id="455a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="455a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="455a3-105">Обновление [контента типа][контента.]</span><span class="sxs-lookup"><span data-stu-id="455a3-105">Update a [content type][contentType].</span></span>
  

## <a name="permissions"></a><span data-ttu-id="455a3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="455a3-106">Permissions</span></span>

  

<span data-ttu-id="455a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="455a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="455a3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="455a3-109">Permission type</span></span> | <span data-ttu-id="455a3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="455a3-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="455a3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="455a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="455a3-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="455a3-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="455a3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="455a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="455a3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="455a3-114">Not supported.</span></span> |
|<span data-ttu-id="455a3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="455a3-115">Application</span></span> |<span data-ttu-id="455a3-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="455a3-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="455a3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="455a3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="455a3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="455a3-118">Request headers</span></span>
|<span data-ttu-id="455a3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="455a3-119">Name</span></span>|<span data-ttu-id="455a3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="455a3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="455a3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="455a3-121">Authorization</span></span>|<span data-ttu-id="455a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="455a3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="455a3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="455a3-124">Content-Type</span></span>|<span data-ttu-id="455a3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="455a3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="455a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="455a3-127">Request body</span></span>

<span data-ttu-id="455a3-128">В теле запроса поставляем представление JSON ресурса [contentType][] для обновления.</span><span class="sxs-lookup"><span data-stu-id="455a3-128">In the request body, supply a JSON representation of the [contentType][] resource to update.</span></span>  

## <a name="response"></a><span data-ttu-id="455a3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="455a3-129">Response</span></span>

<span data-ttu-id="455a3-130">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект contentType][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="455a3-130">If successful, this method returns a `200 OK` response code and an updated [contentType][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="455a3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="455a3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="455a3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="455a3-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contenttype"
}
-->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
Content-Type: application/json

{
    "name": "updatedCt",
    "documentSet": {
        "shouldPrefixNameToFile": true,
        "allowedContentTypes": [{
            "id": "0x0101",
            "name": "Document"
        }],
        "defaultContents": [{
                "fileName": "a.txt",
                "contentType": {
                    "id": "0x0101"
                }
            },
            {
                "fileName": "b.txt",
                "contentType": {
                    "id": "0x0101"
                }
            }
        ],
        "sharedColumns": [{
                "name": "Description",
                "id": "cbb92da4-fd46-4c7d-af6c-3128c2a5576e"
            },
            {
                "name": "Address",
                "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50"
            }
        ],
        "welcomePageColumns": [{
            "name": "Address",
            "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50"
        }]
    }
}

```

### <a name="response"></a><span data-ttu-id="455a3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="455a3-133">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0x0101009B237E76EF94DC49B4E58139041E7C60",
    "description": "",
    "eTag": "\"7\"",
    "group": "Custom Content Types",
    "hidden": false,
    "name": "testdoc",
    "parentId": "0x0101",
    "base": {
        "id": "0x0101",
        "name": "Document"
    }
}

```

[contentType]: ../resources/contentType.md
