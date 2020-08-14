---
title: Создание printJob
description: Создание нового метода printJob для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2236e366e18941d81edcf1d2bdb4d4bf9b9823dd
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673748"
---
# <a name="create-printjob"></a><span data-ttu-id="ad78e-103">Создание printJob</span><span class="sxs-lookup"><span data-stu-id="ad78e-103">Create printJob</span></span>

<span data-ttu-id="ad78e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad78e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad78e-105">Создание нового [метода printJob](../resources/printJob.md) для [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="ad78e-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ad78e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad78e-106">Permissions</span></span>
<span data-ttu-id="ad78e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad78e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ad78e-109">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="ad78e-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span> <span data-ttu-id="ad78e-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="ad78e-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ad78e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad78e-111">Permission type</span></span> | <span data-ttu-id="ad78e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad78e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ad78e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad78e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ad78e-114">PrintJob. Реадвритебасик, PrintJob. ReadWrite, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad78e-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="ad78e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad78e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad78e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad78e-116">Not Supported.</span></span>|
|<span data-ttu-id="ad78e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad78e-117">Application</span></span>| <span data-ttu-id="ad78e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad78e-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad78e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad78e-119">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="ad78e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad78e-120">Request headers</span></span>
| <span data-ttu-id="ad78e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ad78e-121">Name</span></span>      |<span data-ttu-id="ad78e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ad78e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad78e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad78e-123">Authorization</span></span> | <span data-ttu-id="ad78e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad78e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad78e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad78e-126">Content-type</span></span>  | <span data-ttu-id="ad78e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad78e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad78e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad78e-129">Request body</span></span>
<span data-ttu-id="ad78e-130">В тексте запроса добавьте представление объекта [printJob](../resources/printjob.md) в формате JSON, включая один объект [printDocument](../resources/printDocument.md) .</span><span class="sxs-lookup"><span data-stu-id="ad78e-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object, including one [printDocument](../resources/printDocument.md) object.</span></span> <span data-ttu-id="ad78e-131">Задания и идентификаторы документов устанавливаются автоматически во время создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad78e-131">The job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="ad78e-132">Теперь для универсальной печати поддерживается только один **printDocument** для каждого объекта **printJob** .</span><span class="sxs-lookup"><span data-stu-id="ad78e-132">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="ad78e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad78e-133">Response</span></span>
<span data-ttu-id="ad78e-134">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [printJob](../resources/printjob.md) и связанный с [printDocument](../resources/printDocument.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad78e-134">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="ad78e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ad78e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad78e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad78e-136">Request</span></span>
<span data-ttu-id="ad78e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad78e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad78e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad78e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="javascript"></a>[<span data-ttu-id="ad78e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad78e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad78e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad78e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ad78e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad78e-141">Response</span></span>
<span data-ttu-id="ad78e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad78e-142">The following is an example of the response.</span></span>
><span data-ttu-id="ad78e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad78e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 425

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```
