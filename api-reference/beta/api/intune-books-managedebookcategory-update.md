---
title: Обновление Манажедебуккатегори
description: Обновление свойств объекта Манажедебуккатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dad9d166fafb2ad945c99def4280e0948790ac4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690198"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="d027f-103">Обновление Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="d027f-103">Update managedEBookCategory</span></span>

<span data-ttu-id="d027f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d027f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d027f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d027f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d027f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d027f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d027f-107">Обновление свойств объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d027f-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d027f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d027f-108">Prerequisites</span></span>
<span data-ttu-id="d027f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d027f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d027f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d027f-111">Permission type</span></span>|<span data-ttu-id="d027f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d027f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d027f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d027f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d027f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d027f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d027f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d027f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d027f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d027f-116">Not supported.</span></span>|
|<span data-ttu-id="d027f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d027f-117">Application</span></span>|<span data-ttu-id="d027f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d027f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d027f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d027f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="d027f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d027f-120">Request headers</span></span>
|<span data-ttu-id="d027f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d027f-121">Header</span></span>|<span data-ttu-id="d027f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d027f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d027f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d027f-123">Authorization</span></span>|<span data-ttu-id="d027f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d027f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d027f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d027f-125">Accept</span></span>|<span data-ttu-id="d027f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d027f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d027f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d027f-127">Request body</span></span>
<span data-ttu-id="d027f-128">В тексте запроса добавьте представление объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d027f-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="d027f-129">В следующей таблице приведены свойства, необходимые при создании [манажедебуккатегори](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="d027f-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="d027f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d027f-130">Property</span></span>|<span data-ttu-id="d027f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d027f-131">Type</span></span>|<span data-ttu-id="d027f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d027f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d027f-133">id</span><span class="sxs-lookup"><span data-stu-id="d027f-133">id</span></span>|<span data-ttu-id="d027f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d027f-134">String</span></span>|<span data-ttu-id="d027f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d027f-135">The key of the entity.</span></span>|
|<span data-ttu-id="d027f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d027f-136">displayName</span></span>|<span data-ttu-id="d027f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d027f-137">String</span></span>|<span data-ttu-id="d027f-138">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="d027f-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="d027f-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d027f-139">lastModifiedDateTime</span></span>|<span data-ttu-id="d027f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d027f-140">DateTimeOffset</span></span>|<span data-ttu-id="d027f-141">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="d027f-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d027f-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="d027f-142">Response</span></span>
<span data-ttu-id="d027f-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d027f-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d027f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d027f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d027f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d027f-145">Request</span></span>
<span data-ttu-id="d027f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d027f-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d027f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d027f-147">Response</span></span>
<span data-ttu-id="d027f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d027f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





