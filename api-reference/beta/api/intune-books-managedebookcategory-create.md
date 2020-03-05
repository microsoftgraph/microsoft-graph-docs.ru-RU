---
title: Создание Манажедебуккатегори
description: Создание нового объекта Манажедебуккатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 661febade05a63291bc502cc8c2f3194b93491a3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450302"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="e1f6f-103">Создание Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="e1f6f-103">Create managedEBookCategory</span></span>

<span data-ttu-id="e1f6f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e1f6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1f6f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1f6f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1f6f-107">Создание нового объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="e1f6f-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1f6f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1f6f-108">Prerequisites</span></span>
<span data-ttu-id="e1f6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1f6f-111">Permission type</span></span>|<span data-ttu-id="e1f6f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1f6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1f6f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1f6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1f6f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1f6f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1f6f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1f6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1f6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-116">Not supported.</span></span>|
|<span data-ttu-id="e1f6f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1f6f-117">Application</span></span>|<span data-ttu-id="e1f6f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1f6f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1f6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1f6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="e1f6f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e1f6f-120">Request headers</span></span>
|<span data-ttu-id="e1f6f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1f6f-121">Header</span></span>|<span data-ttu-id="e1f6f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1f6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1f6f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1f6f-123">Authorization</span></span>|<span data-ttu-id="e1f6f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1f6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1f6f-125">Accept</span></span>|<span data-ttu-id="e1f6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1f6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1f6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1f6f-127">Request body</span></span>
<span data-ttu-id="e1f6f-128">В тексте запроса добавьте представление объекта Манажедебуккатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="e1f6f-129">В следующей таблице приведены свойства, необходимые при создании Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="e1f6f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1f6f-130">Property</span></span>|<span data-ttu-id="e1f6f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1f6f-131">Type</span></span>|<span data-ttu-id="e1f6f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1f6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1f6f-133">id</span><span class="sxs-lookup"><span data-stu-id="e1f6f-133">id</span></span>|<span data-ttu-id="e1f6f-134">String</span><span class="sxs-lookup"><span data-stu-id="e1f6f-134">String</span></span>|<span data-ttu-id="e1f6f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-135">The key of the entity.</span></span>|
|<span data-ttu-id="e1f6f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e1f6f-136">displayName</span></span>|<span data-ttu-id="e1f6f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e1f6f-137">String</span></span>|<span data-ttu-id="e1f6f-138">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="e1f6f-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1f6f-139">lastModifiedDateTime</span></span>|<span data-ttu-id="e1f6f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1f6f-140">DateTimeOffset</span></span>|<span data-ttu-id="e1f6f-141">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="e1f6f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1f6f-142">Response</span></span>
<span data-ttu-id="e1f6f-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1f6f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e1f6f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1f6f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1f6f-145">Request</span></span>
<span data-ttu-id="e1f6f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="e1f6f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1f6f-147">Response</span></span>
<span data-ttu-id="e1f6f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1f6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





