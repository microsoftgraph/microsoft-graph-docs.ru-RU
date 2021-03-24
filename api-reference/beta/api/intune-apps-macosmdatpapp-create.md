---
title: Создание macOSMdatpApp
description: Создание нового объекта macOSMdatpApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8035395216ac28bf402aa66f5cc34adf857eba5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140492"
---
# <a name="create-macosmdatpapp"></a><span data-ttu-id="c3b2d-103">Создание macOSMdatpApp</span><span class="sxs-lookup"><span data-stu-id="c3b2d-103">Create macOSMdatpApp</span></span>

<span data-ttu-id="c3b2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3b2d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3b2d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3b2d-107">Создание нового [объекта macOSMdatpApp.](../resources/intune-apps-macosmdatpapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3b2d-107">Create a new [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3b2d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3b2d-108">Prerequisites</span></span>
<span data-ttu-id="c3b2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3b2d-111">Permission type</span></span>|<span data-ttu-id="c3b2d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3b2d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3b2d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3b2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3b2d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3b2d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3b2d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3b2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3b2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-116">Not supported.</span></span>|
|<span data-ttu-id="c3b2d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3b2d-117">Application</span></span>|<span data-ttu-id="c3b2d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3b2d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3b2d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3b2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c3b2d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3b2d-120">Request headers</span></span>
|<span data-ttu-id="c3b2d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3b2d-121">Header</span></span>|<span data-ttu-id="c3b2d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3b2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3b2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3b2d-123">Authorization</span></span>|<span data-ttu-id="c3b2d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3b2d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3b2d-125">Accept</span></span>|<span data-ttu-id="c3b2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3b2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3b2d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3b2d-127">Request body</span></span>
<span data-ttu-id="c3b2d-128">В теле запроса поставляем представление JSON для объекта macOSMdatpApp.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-128">In the request body, supply a JSON representation for the macOSMdatpApp object.</span></span>

<span data-ttu-id="c3b2d-129">В следующей таблице показаны свойства, необходимые при создании macOSMdatpApp.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-129">The following table shows the properties that are required when you create the macOSMdatpApp.</span></span>

|<span data-ttu-id="c3b2d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3b2d-130">Property</span></span>|<span data-ttu-id="c3b2d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3b2d-131">Type</span></span>|<span data-ttu-id="c3b2d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3b2d-133">id</span><span class="sxs-lookup"><span data-stu-id="c3b2d-133">id</span></span>|<span data-ttu-id="c3b2d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c3b2d-134">String</span></span>|<span data-ttu-id="c3b2d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-135">Key of the entity.</span></span> <span data-ttu-id="c3b2d-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c3b2d-137">displayName</span></span>|<span data-ttu-id="c3b2d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c3b2d-138">String</span></span>|<span data-ttu-id="c3b2d-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c3b2d-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-141">description</span><span class="sxs-lookup"><span data-stu-id="c3b2d-141">description</span></span>|<span data-ttu-id="c3b2d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="c3b2d-142">String</span></span>|<span data-ttu-id="c3b2d-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-143">The description of the app.</span></span> <span data-ttu-id="c3b2d-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c3b2d-145">publisher</span></span>|<span data-ttu-id="c3b2d-146">String</span><span class="sxs-lookup"><span data-stu-id="c3b2d-146">String</span></span>|<span data-ttu-id="c3b2d-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-147">The publisher of the app.</span></span> <span data-ttu-id="c3b2d-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c3b2d-149">largeIcon</span></span>|[<span data-ttu-id="c3b2d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c3b2d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c3b2d-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c3b2d-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3b2d-153">createdDateTime</span></span>|<span data-ttu-id="c3b2d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3b2d-154">DateTimeOffset</span></span>|<span data-ttu-id="c3b2d-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-155">The date and time the app was created.</span></span> <span data-ttu-id="c3b2d-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3b2d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c3b2d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3b2d-158">DateTimeOffset</span></span>|<span data-ttu-id="c3b2d-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c3b2d-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c3b2d-161">isFeatured</span></span>|<span data-ttu-id="c3b2d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b2d-162">Boolean</span></span>|<span data-ttu-id="c3b2d-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c3b2d-164">privacyInformationUrl</span></span>|<span data-ttu-id="c3b2d-165">String</span><span class="sxs-lookup"><span data-stu-id="c3b2d-165">String</span></span>|<span data-ttu-id="c3b2d-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-166">The privacy statement Url.</span></span> <span data-ttu-id="c3b2d-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c3b2d-168">informationUrl</span></span>|<span data-ttu-id="c3b2d-169">String</span><span class="sxs-lookup"><span data-stu-id="c3b2d-169">String</span></span>|<span data-ttu-id="c3b2d-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-170">The more information Url.</span></span> <span data-ttu-id="c3b2d-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-172">owner</span><span class="sxs-lookup"><span data-stu-id="c3b2d-172">owner</span></span>|<span data-ttu-id="c3b2d-173">String</span><span class="sxs-lookup"><span data-stu-id="c3b2d-173">String</span></span>|<span data-ttu-id="c3b2d-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-174">The owner of the app.</span></span> <span data-ttu-id="c3b2d-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-176">developer</span><span class="sxs-lookup"><span data-stu-id="c3b2d-176">developer</span></span>|<span data-ttu-id="c3b2d-177">String</span><span class="sxs-lookup"><span data-stu-id="c3b2d-177">String</span></span>|<span data-ttu-id="c3b2d-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-178">The developer of the app.</span></span> <span data-ttu-id="c3b2d-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-180">notes</span><span class="sxs-lookup"><span data-stu-id="c3b2d-180">notes</span></span>|<span data-ttu-id="c3b2d-181">String</span><span class="sxs-lookup"><span data-stu-id="c3b2d-181">String</span></span>|<span data-ttu-id="c3b2d-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-182">Notes for the app.</span></span> <span data-ttu-id="c3b2d-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c3b2d-184">uploadState</span></span>|<span data-ttu-id="c3b2d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b2d-185">Int32</span></span>|<span data-ttu-id="c3b2d-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-186">The upload state.</span></span> <span data-ttu-id="c3b2d-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="c3b2d-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="c3b2d-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="c3b2d-189">publishingState</span></span>|[<span data-ttu-id="c3b2d-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c3b2d-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c3b2d-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-191">The publishing state for the app.</span></span> <span data-ttu-id="c3b2d-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c3b2d-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="c3b2d-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c3b2d-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c3b2d-195">isAssigned</span></span>|<span data-ttu-id="c3b2d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3b2d-196">Boolean</span></span>|<span data-ttu-id="c3b2d-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c3b2d-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3b2d-199">roleScopeTagIds</span></span>|<span data-ttu-id="c3b2d-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c3b2d-200">String collection</span></span>|<span data-ttu-id="c3b2d-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c3b2d-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c3b2d-203">dependentAppCount</span></span>|<span data-ttu-id="c3b2d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b2d-204">Int32</span></span>|<span data-ttu-id="c3b2d-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c3b2d-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="c3b2d-207">supersedingAppCount</span></span>|<span data-ttu-id="c3b2d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b2d-208">Int32</span></span>|<span data-ttu-id="c3b2d-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="c3b2d-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c3b2d-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="c3b2d-211">supersededAppCount</span></span>|<span data-ttu-id="c3b2d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="c3b2d-212">Int32</span></span>|<span data-ttu-id="c3b2d-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="c3b2d-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c3b2d-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c3b2d-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b2d-215">Response</span></span>
<span data-ttu-id="c3b2d-216">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-216">If successful, this method returns a `201 Created` response code and a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3b2d-217">Пример</span><span class="sxs-lookup"><span data-stu-id="c3b2d-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3b2d-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3b2d-218">Request</span></span>
<span data-ttu-id="c3b2d-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "supersedingAppCount": 3,
  "supersededAppCount": 2
}
```

### <a name="response"></a><span data-ttu-id="c3b2d-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b2d-220">Response</span></span>
<span data-ttu-id="c3b2d-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3b2d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
  "id": "2963b007-b007-2963-07b0-632907b06329",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "supersedingAppCount": 3,
  "supersededAppCount": 2
}
```




