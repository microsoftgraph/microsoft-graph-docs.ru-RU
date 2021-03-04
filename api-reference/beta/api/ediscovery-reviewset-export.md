---
title: 'reviewSet: экспорт'
description: Инициировать экспорт из reviewSet.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7ee3744470cf5fac31abad2d4cc53ba47a0feca5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446972"
---
# <a name="reviewset-export"></a><span data-ttu-id="f81b8-103">reviewSet: экспорт</span><span class="sxs-lookup"><span data-stu-id="f81b8-103">reviewSet: export</span></span>

<span data-ttu-id="f81b8-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f81b8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f81b8-105">Инициировать экспорт из **reviewSet**.</span><span class="sxs-lookup"><span data-stu-id="f81b8-105">Initiate an export from a **reviewSet**.</span></span>  <span data-ttu-id="f81b8-106">Дополнительные сведения см. [в материале Export documents from a review set in Advanced eDiscovery.](/microsoft-365/compliance/export-documents-from-review-set)</span><span class="sxs-lookup"><span data-stu-id="f81b8-106">For details, see [Export documents from a review set in Advanced eDiscovery](/microsoft-365/compliance/export-documents-from-review-set).</span></span>

## <a name="permissions"></a><span data-ttu-id="f81b8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f81b8-107">Permissions</span></span>

<span data-ttu-id="f81b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f81b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f81b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f81b8-110">Permission type</span></span>|<span data-ttu-id="f81b8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f81b8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f81b8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f81b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f81b8-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f81b8-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f81b8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f81b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f81b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f81b8-115">Not supported.</span></span>|
|<span data-ttu-id="f81b8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f81b8-116">Application</span></span>|<span data-ttu-id="f81b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f81b8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f81b8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f81b8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewsets/{reviewsetId}/export
```

## <a name="request-headers"></a><span data-ttu-id="f81b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f81b8-119">Request headers</span></span>

|<span data-ttu-id="f81b8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f81b8-120">Name</span></span>|<span data-ttu-id="f81b8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f81b8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f81b8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f81b8-122">Authorization</span></span>|<span data-ttu-id="f81b8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f81b8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f81b8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f81b8-125">Content-Type</span></span>|<span data-ttu-id="f81b8-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f81b8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f81b8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f81b8-128">Request body</span></span>

<span data-ttu-id="f81b8-129">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="f81b8-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="f81b8-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f81b8-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f81b8-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="f81b8-131">Parameter</span></span>|<span data-ttu-id="f81b8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f81b8-132">Type</span></span>|<span data-ttu-id="f81b8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f81b8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f81b8-134">outputName</span><span class="sxs-lookup"><span data-stu-id="f81b8-134">outputName</span></span>|<span data-ttu-id="f81b8-135">String</span><span class="sxs-lookup"><span data-stu-id="f81b8-135">String</span></span>| <span data-ttu-id="f81b8-136">Имя экспорта.</span><span class="sxs-lookup"><span data-stu-id="f81b8-136">Name of the export.</span></span> <span data-ttu-id="f81b8-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f81b8-137">Required.</span></span> |
|<span data-ttu-id="f81b8-138">description</span><span class="sxs-lookup"><span data-stu-id="f81b8-138">description</span></span>|<span data-ttu-id="f81b8-139">String</span><span class="sxs-lookup"><span data-stu-id="f81b8-139">String</span></span>| <span data-ttu-id="f81b8-140">Описание экспорта</span><span class="sxs-lookup"><span data-stu-id="f81b8-140">Description of the export</span></span> |
|<span data-ttu-id="f81b8-141">azureBlobContainer</span><span class="sxs-lookup"><span data-stu-id="f81b8-141">azureBlobContainer</span></span>|<span data-ttu-id="f81b8-142">String</span><span class="sxs-lookup"><span data-stu-id="f81b8-142">String</span></span>| <span data-ttu-id="f81b8-143">При экспорте в собственную учетную запись хранения Azure это URL-адрес контейнера.</span><span class="sxs-lookup"><span data-stu-id="f81b8-143">When exporting to your own Azure storage account, this is the container URL.</span></span> |
|<span data-ttu-id="f81b8-144">azureBlobToken</span><span class="sxs-lookup"><span data-stu-id="f81b8-144">azureBlobToken</span></span>|<span data-ttu-id="f81b8-145">String</span><span class="sxs-lookup"><span data-stu-id="f81b8-145">String</span></span>| <span data-ttu-id="f81b8-146">При экспорте на собственную учетную запись хранения Azure маркер SAS для URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="f81b8-146">When exporting to your own Azure storage account, SAS token for the container URL.</span></span> |
|<span data-ttu-id="f81b8-147">ExportOptions</span><span class="sxs-lookup"><span data-stu-id="f81b8-147">exportOptions</span></span>| [<span data-ttu-id="f81b8-148">microsoft.graph.ediscovery.exportOptions</span><span class="sxs-lookup"><span data-stu-id="f81b8-148">microsoft.graph.ediscovery.exportOptions</span></span>](../resources/ediscovery-caseexportoperation.md#exportoptions-values) |<span data-ttu-id="f81b8-149">Указывает параметры, которые контролируют формат экспорта.</span><span class="sxs-lookup"><span data-stu-id="f81b8-149">Specifies options that control the format of the export.</span></span> <span data-ttu-id="f81b8-150">Возможные значения: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span><span class="sxs-lookup"><span data-stu-id="f81b8-150">Possible values are: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span></span>|
|<span data-ttu-id="f81b8-151">exportStructure</span><span class="sxs-lookup"><span data-stu-id="f81b8-151">exportStructure</span></span>|[<span data-ttu-id="f81b8-152">microsoft.graph.ediscovery.exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="f81b8-152">microsoft.graph.ediscovery.exportFileStructure</span></span>](../resources/ediscovery-caseexportoperation.md#exportfilestructure-values)| <span data-ttu-id="f81b8-153">Параметры, которые контролируют структуру файлов и упаковку экспорта.</span><span class="sxs-lookup"><span data-stu-id="f81b8-153">Options that control file structure and packaging of the export.</span></span> <span data-ttu-id="f81b8-154">Возможные значения: `none`, `directory`, `pst`.</span><span class="sxs-lookup"><span data-stu-id="f81b8-154">Possible values are: `none`, `directory`, `pst`.</span></span>|

## <a name="response"></a><span data-ttu-id="f81b8-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f81b8-155">Response</span></span>

<span data-ttu-id="f81b8-156">Если экспорт успешно запущен, это действие возвращает код `202 Accepted` ответа.</span><span class="sxs-lookup"><span data-stu-id="f81b8-156">If the export is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="f81b8-157">В ответе также будет содержаться `Location` заглавный загот, содержащий расположение [caseExportOperation,](../resources/ediscovery-caseexportoperation.md) созданного для обработки экспорта.</span><span class="sxs-lookup"><span data-stu-id="f81b8-157">The response will also contain a `Location` header, which contains the location of the [caseExportOperation](../resources/ediscovery-caseexportoperation.md) that was created to handle the export.</span></span> <span data-ttu-id="f81b8-158">Проверьте состояние экспортной операции, сделав запрос GET в расположение, после успешного завершения состояние [изменится](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) на `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="f81b8-158">Check the status of the export operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="f81b8-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="f81b8-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f81b8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="f81b8-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reviewset_export"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/reviewsets/e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc/export
Content-Type: application/json
Content-length: 186

{
  "outputName": "2020-12-06 Contoso investigation export",
  "description": "Export for the Contoso investigation",
  "exportOptions": "originalFiles,fileInfo,tags",
  "exportStructure": "directory"
}
```

### <a name="response"></a><span data-ttu-id="f81b8-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f81b8-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 3ec98906-7187-927e-5203-2ed4533175c6,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/operations('2ad2da7c7dbb404abfbbb28b7b6babd6'),
request-id: 9e6b9230-113c-49de-8f7d-ecb90d35b0de
```
