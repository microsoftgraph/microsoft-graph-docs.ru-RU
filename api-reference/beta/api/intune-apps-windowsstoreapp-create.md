---
title: Создание Виндовсстореапп
description: Создание нового объекта Виндовсстореапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5b5784036cfe839e700c020b42848cff42ab929
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724391"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="a84fa-103">Создание Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="a84fa-103">Create windowsStoreApp</span></span>

<span data-ttu-id="a84fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a84fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a84fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a84fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a84fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a84fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a84fa-107">Создание нового объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a84fa-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a84fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a84fa-108">Prerequisites</span></span>
<span data-ttu-id="a84fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a84fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a84fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a84fa-111">Permission type</span></span>|<span data-ttu-id="a84fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a84fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a84fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a84fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a84fa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a84fa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a84fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a84fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a84fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a84fa-116">Not supported.</span></span>|
|<span data-ttu-id="a84fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a84fa-117">Application</span></span>|<span data-ttu-id="a84fa-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a84fa-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a84fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a84fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a84fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a84fa-120">Request headers</span></span>
|<span data-ttu-id="a84fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a84fa-121">Header</span></span>|<span data-ttu-id="a84fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a84fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a84fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a84fa-123">Authorization</span></span>|<span data-ttu-id="a84fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a84fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a84fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a84fa-125">Accept</span></span>|<span data-ttu-id="a84fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a84fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a84fa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a84fa-127">Request body</span></span>
<span data-ttu-id="a84fa-128">В тексте запроса добавьте представление объекта Виндовсстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a84fa-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="a84fa-129">В следующей таблице приведены свойства, необходимые при создании Виндовсстореапп.</span><span class="sxs-lookup"><span data-stu-id="a84fa-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="a84fa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a84fa-130">Property</span></span>|<span data-ttu-id="a84fa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a84fa-131">Type</span></span>|<span data-ttu-id="a84fa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a84fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a84fa-133">id</span><span class="sxs-lookup"><span data-stu-id="a84fa-133">id</span></span>|<span data-ttu-id="a84fa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a84fa-134">String</span></span>|<span data-ttu-id="a84fa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a84fa-135">Key of the entity.</span></span> <span data-ttu-id="a84fa-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a84fa-137">displayName</span></span>|<span data-ttu-id="a84fa-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a84fa-138">String</span></span>|<span data-ttu-id="a84fa-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a84fa-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a84fa-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-141">description</span><span class="sxs-lookup"><span data-stu-id="a84fa-141">description</span></span>|<span data-ttu-id="a84fa-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a84fa-142">String</span></span>|<span data-ttu-id="a84fa-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-143">The description of the app.</span></span> <span data-ttu-id="a84fa-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a84fa-145">publisher</span></span>|<span data-ttu-id="a84fa-146">String</span><span class="sxs-lookup"><span data-stu-id="a84fa-146">String</span></span>|<span data-ttu-id="a84fa-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-147">The publisher of the app.</span></span> <span data-ttu-id="a84fa-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a84fa-149">largeIcon</span></span>|[<span data-ttu-id="a84fa-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a84fa-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a84fa-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a84fa-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a84fa-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a84fa-153">createdDateTime</span></span>|<span data-ttu-id="a84fa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a84fa-154">DateTimeOffset</span></span>|<span data-ttu-id="a84fa-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-155">The date and time the app was created.</span></span> <span data-ttu-id="a84fa-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a84fa-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a84fa-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a84fa-158">DateTimeOffset</span></span>|<span data-ttu-id="a84fa-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a84fa-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a84fa-161">isFeatured</span></span>|<span data-ttu-id="a84fa-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a84fa-162">Boolean</span></span>|<span data-ttu-id="a84fa-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a84fa-164">privacyInformationUrl</span></span>|<span data-ttu-id="a84fa-165">String</span><span class="sxs-lookup"><span data-stu-id="a84fa-165">String</span></span>|<span data-ttu-id="a84fa-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a84fa-166">The privacy statement Url.</span></span> <span data-ttu-id="a84fa-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a84fa-168">informationUrl</span></span>|<span data-ttu-id="a84fa-169">String</span><span class="sxs-lookup"><span data-stu-id="a84fa-169">String</span></span>|<span data-ttu-id="a84fa-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a84fa-170">The more information Url.</span></span> <span data-ttu-id="a84fa-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-172">owner</span><span class="sxs-lookup"><span data-stu-id="a84fa-172">owner</span></span>|<span data-ttu-id="a84fa-173">String</span><span class="sxs-lookup"><span data-stu-id="a84fa-173">String</span></span>|<span data-ttu-id="a84fa-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-174">The owner of the app.</span></span> <span data-ttu-id="a84fa-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-176">developer</span><span class="sxs-lookup"><span data-stu-id="a84fa-176">developer</span></span>|<span data-ttu-id="a84fa-177">String</span><span class="sxs-lookup"><span data-stu-id="a84fa-177">String</span></span>|<span data-ttu-id="a84fa-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-178">The developer of the app.</span></span> <span data-ttu-id="a84fa-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-180">notes</span><span class="sxs-lookup"><span data-stu-id="a84fa-180">notes</span></span>|<span data-ttu-id="a84fa-181">String</span><span class="sxs-lookup"><span data-stu-id="a84fa-181">String</span></span>|<span data-ttu-id="a84fa-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-182">Notes for the app.</span></span> <span data-ttu-id="a84fa-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a84fa-184">uploadState</span></span>|<span data-ttu-id="a84fa-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a84fa-185">Int32</span></span>|<span data-ttu-id="a84fa-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="a84fa-186">The upload state.</span></span> <span data-ttu-id="a84fa-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="a84fa-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a84fa-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a84fa-189">publishingState</span></span>|[<span data-ttu-id="a84fa-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a84fa-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a84fa-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-191">The publishing state for the app.</span></span> <span data-ttu-id="a84fa-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a84fa-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a84fa-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a84fa-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a84fa-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a84fa-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a84fa-195">isAssigned</span></span>|<span data-ttu-id="a84fa-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a84fa-196">Boolean</span></span>|<span data-ttu-id="a84fa-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="a84fa-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a84fa-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a84fa-199">roleScopeTagIds</span></span>|<span data-ttu-id="a84fa-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a84fa-200">String collection</span></span>|<span data-ttu-id="a84fa-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a84fa-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a84fa-203">dependentAppCount</span></span>|<span data-ttu-id="a84fa-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a84fa-204">Int32</span></span>|<span data-ttu-id="a84fa-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="a84fa-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a84fa-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a84fa-207">supersedingAppCount</span></span>|<span data-ttu-id="a84fa-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a84fa-208">Int32</span></span>|<span data-ttu-id="a84fa-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="a84fa-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a84fa-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a84fa-211">supersededAppCount</span></span>|<span data-ttu-id="a84fa-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a84fa-212">Int32</span></span>|<span data-ttu-id="a84fa-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="a84fa-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a84fa-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a84fa-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a84fa-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a84fa-215">appStoreUrl</span></span>|<span data-ttu-id="a84fa-216">String</span><span class="sxs-lookup"><span data-stu-id="a84fa-216">String</span></span>|<span data-ttu-id="a84fa-217">URL-адрес хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="a84fa-217">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="a84fa-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="a84fa-218">Response</span></span>
<span data-ttu-id="a84fa-219">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a84fa-219">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a84fa-220">Пример</span><span class="sxs-lookup"><span data-stu-id="a84fa-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="a84fa-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="a84fa-221">Request</span></span>
<span data-ttu-id="a84fa-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a84fa-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 825

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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
  "supersededAppCount": 2,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="a84fa-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="a84fa-223">Response</span></span>
<span data-ttu-id="a84fa-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a84fa-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 997

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
  "supersededAppCount": 2,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





