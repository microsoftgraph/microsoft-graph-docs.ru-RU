---
title: Обновление managedEBookCategory
description: Обновление свойства объекта managedEBookCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 236159e64bccd0eb5ce03de0c04d8b5fdf99b47d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990909"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="e384b-103">Обновление managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="e384b-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="e384b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e384b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e384b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e384b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e384b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e384b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e384b-107">Обновление свойства объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="e384b-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e384b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e384b-108">Prerequisites</span></span>
<span data-ttu-id="e384b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e384b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e384b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e384b-111">Permission type</span></span>|<span data-ttu-id="e384b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e384b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e384b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e384b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e384b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e384b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e384b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e384b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e384b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e384b-116">Not supported.</span></span>|
|<span data-ttu-id="e384b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e384b-117">Application</span></span>|<span data-ttu-id="e384b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e384b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e384b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e384b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="e384b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e384b-120">Request headers</span></span>
|<span data-ttu-id="e384b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e384b-121">Header</span></span>|<span data-ttu-id="e384b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e384b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e384b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e384b-123">Authorization</span></span>|<span data-ttu-id="e384b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e384b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e384b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e384b-125">Accept</span></span>|<span data-ttu-id="e384b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e384b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e384b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e384b-127">Request body</span></span>
<span data-ttu-id="e384b-128">В тексте запроса укажите представление JSON для объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="e384b-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="e384b-129">В следующей таблице показаны свойства, которые необходимы для создания [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e384b-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="e384b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e384b-130">Property</span></span>|<span data-ttu-id="e384b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e384b-131">Type</span></span>|<span data-ttu-id="e384b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e384b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e384b-133">id</span><span class="sxs-lookup"><span data-stu-id="e384b-133">id</span></span>|<span data-ttu-id="e384b-134">String</span><span class="sxs-lookup"><span data-stu-id="e384b-134">String</span></span>|<span data-ttu-id="e384b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e384b-135">The key of the entity.</span></span>|
|<span data-ttu-id="e384b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e384b-136">displayName</span></span>|<span data-ttu-id="e384b-137">String</span><span class="sxs-lookup"><span data-stu-id="e384b-137">String</span></span>|<span data-ttu-id="e384b-138">Имя категории электронная книга.</span><span class="sxs-lookup"><span data-stu-id="e384b-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="e384b-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e384b-139">lastModifiedDateTime</span></span>|<span data-ttu-id="e384b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e384b-140">DateTimeOffset</span></span>|<span data-ttu-id="e384b-141">Дата и время последнего изменения ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="e384b-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="e384b-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="e384b-142">Response</span></span>
<span data-ttu-id="e384b-143">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managedEBookCategory](../resources/intune-books-managedebookcategory.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e384b-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e384b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e384b-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="e384b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e384b-145">Request</span></span>
<span data-ttu-id="e384b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e384b-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e384b-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="e384b-147">Response</span></span>
<span data-ttu-id="e384b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e384b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





