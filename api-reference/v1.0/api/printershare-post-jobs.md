---
title: Создание printJob для принтераShare
description: Создайте новый printJob для принтераShare.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9dafcee89de7352c2887ffd13788d5f1bcda202f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517944"
---
# <a name="create-printjob-for-a-printershare"></a><span data-ttu-id="a1114-103">Создание printJob для принтераShare</span><span class="sxs-lookup"><span data-stu-id="a1114-103">Create printJob for a printerShare</span></span>
<span data-ttu-id="a1114-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1114-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a1114-105">Создайте новый [printJob](../resources/printJob.md) для [принтераShare](../resources/printerShare.md).</span><span class="sxs-lookup"><span data-stu-id="a1114-105">Create a new [printJob](../resources/printJob.md) for a [printerShare](../resources/printerShare.md).</span></span> 

<span data-ttu-id="a1114-106">Также создается новый [printDocument,](../resources/printDocument.md) связанный с printJob.</span><span class="sxs-lookup"><span data-stu-id="a1114-106">Also creates a new [printDocument](../resources/printDocument.md) associated with the printJob.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1114-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1114-107">Permissions</span></span>
<span data-ttu-id="a1114-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a1114-110">Помимо следующих разрешений, пользователь или клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение, дава которое предоставляет доступ [get printerShare.](printerShare-get.md)</span><span class="sxs-lookup"><span data-stu-id="a1114-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printerShare](printerShare-get.md) access.</span></span> <span data-ttu-id="a1114-111">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a1114-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a1114-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1114-112">Permission type</span></span> | <span data-ttu-id="a1114-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1114-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a1114-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1114-114">Delegated (work or school account)</span></span>| <span data-ttu-id="a1114-115">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1114-115">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="a1114-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1114-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1114-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1114-117">Not Supported.</span></span>|
|<span data-ttu-id="a1114-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="a1114-118">Application</span></span>| <span data-ttu-id="a1114-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1114-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1114-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1114-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="a1114-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1114-121">Request headers</span></span>
|<span data-ttu-id="a1114-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a1114-122">Name</span></span>|<span data-ttu-id="a1114-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a1114-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a1114-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1114-124">Authorization</span></span>|<span data-ttu-id="a1114-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1114-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a1114-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1114-127">Content-Type</span></span>|<span data-ttu-id="a1114-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1114-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1114-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1114-130">Request body</span></span>
<span data-ttu-id="a1114-131">В теле запроса поставляем представление JSON объекта [printJob.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a1114-131">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="a1114-132">Объект printJob должен содержать только **свойство конфигурации.**</span><span class="sxs-lookup"><span data-stu-id="a1114-132">The printJob object should only contain **configuration** property.</span></span> <span data-ttu-id="a1114-133">Все свойства **конфигурации** являются недействительными.</span><span class="sxs-lookup"><span data-stu-id="a1114-133">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="a1114-134">Все другие поля, включая ИД рабочих мест и документов, устанавливаются автоматически во время создания ресурсов и не должны предоставляться в запросе.</span><span class="sxs-lookup"><span data-stu-id="a1114-134">All other fields, including job and document IDs, are set automatically during resource creation and should not be provided in request.</span></span>

<span data-ttu-id="a1114-135">Сейчас универсальный шрифт поддерживает только одну **печатьDocument на** **объект printJob.**</span><span class="sxs-lookup"><span data-stu-id="a1114-135">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="a1114-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1114-136">Response</span></span>

<span data-ttu-id="a1114-137">В случае успешного выполнения этот метод возвращает код отклика и объект printJob и связанный с ним `201 Created` [шрифтDocument](../resources/printDocument.md) в тексте ответа. [](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a1114-137">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 

## <a name="examples"></a><span data-ttu-id="a1114-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="a1114-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1114-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1114-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printjob_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs
Content-Type: application/json
Content-length: 376

{
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```


### <a name="response"></a><span data-ttu-id="a1114-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1114-140">Response</span></span>
<span data-ttu-id="a1114-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1114-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printJobs/$entity",
  "id": "1825",
  "createdDateTime": "2020-10-14T05:16:49-07:00",
  "isFetchable": false,
  "redirectedFrom": null,
  "redirectedTo": null,
  "createdBy": {
    "id": "{userId}",
    "displayName": "{username}",
    "ipAddress": null,
    "userPrincipalName": "{userupn}"
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet.",
    "isAcquiredByPrinter": false,
    "details": [
      "uploadPending"
    ]
  },
  "configuration": {
    "quality": "medium",
    "dpi": 600,
    "feedOrientation": "longEdgeFirst",
    "orientation": "landscape",
    "duplexMode": "oneSided",
    "copies": 1,
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false,
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    }
  },
  "documents": [
    {
      "id": "1477576d-5dab-4ea9-865c-c0b82cd70bd5",
      "displayName": "",
      "contentType": "",
      "size": 0
    }
  ]
}
```

