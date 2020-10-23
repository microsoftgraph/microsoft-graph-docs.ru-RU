---
title: Создание windowsPhone81AppX
description: Создание нового объекта windowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0dd9057dfa53f67bbec0c3e49d3d209db207672
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709714"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="33f93-103">Создание windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="33f93-103">Create windowsPhone81AppX</span></span>

<span data-ttu-id="33f93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33f93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33f93-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33f93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33f93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33f93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33f93-107">Создание нового объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="33f93-107">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33f93-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33f93-108">Prerequisites</span></span>
<span data-ttu-id="33f93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33f93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33f93-111">Permission type</span></span>|<span data-ttu-id="33f93-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33f93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33f93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33f93-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f93-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="33f93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33f93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33f93-116">Not supported.</span></span>|
|<span data-ttu-id="33f93-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33f93-117">Application</span></span>|<span data-ttu-id="33f93-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f93-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33f93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="33f93-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33f93-120">Request headers</span></span>
|<span data-ttu-id="33f93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33f93-121">Header</span></span>|<span data-ttu-id="33f93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33f93-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33f93-123">Authorization</span></span>|<span data-ttu-id="33f93-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33f93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33f93-125">Accept</span></span>|<span data-ttu-id="33f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f93-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33f93-127">Request body</span></span>
<span data-ttu-id="33f93-128">В тексте запроса добавьте представление объекта windowsPhone81AppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33f93-128">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="33f93-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="33f93-129">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="33f93-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="33f93-130">Property</span></span>|<span data-ttu-id="33f93-131">Тип</span><span class="sxs-lookup"><span data-stu-id="33f93-131">Type</span></span>|<span data-ttu-id="33f93-132">Описание</span><span class="sxs-lookup"><span data-stu-id="33f93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33f93-133">id</span><span class="sxs-lookup"><span data-stu-id="33f93-133">id</span></span>|<span data-ttu-id="33f93-134">Строка</span><span class="sxs-lookup"><span data-stu-id="33f93-134">String</span></span>|<span data-ttu-id="33f93-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33f93-135">Key of the entity.</span></span> <span data-ttu-id="33f93-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-137">displayName</span><span class="sxs-lookup"><span data-stu-id="33f93-137">displayName</span></span>|<span data-ttu-id="33f93-138">Строка</span><span class="sxs-lookup"><span data-stu-id="33f93-138">String</span></span>|<span data-ttu-id="33f93-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="33f93-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="33f93-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-141">description</span><span class="sxs-lookup"><span data-stu-id="33f93-141">description</span></span>|<span data-ttu-id="33f93-142">Строка</span><span class="sxs-lookup"><span data-stu-id="33f93-142">String</span></span>|<span data-ttu-id="33f93-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-143">The description of the app.</span></span> <span data-ttu-id="33f93-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-145">publisher</span><span class="sxs-lookup"><span data-stu-id="33f93-145">publisher</span></span>|<span data-ttu-id="33f93-146">String</span><span class="sxs-lookup"><span data-stu-id="33f93-146">String</span></span>|<span data-ttu-id="33f93-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-147">The publisher of the app.</span></span> <span data-ttu-id="33f93-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="33f93-149">largeIcon</span></span>|[<span data-ttu-id="33f93-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="33f93-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="33f93-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="33f93-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="33f93-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33f93-153">createdDateTime</span></span>|<span data-ttu-id="33f93-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33f93-154">DateTimeOffset</span></span>|<span data-ttu-id="33f93-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-155">The date and time the app was created.</span></span> <span data-ttu-id="33f93-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33f93-157">lastModifiedDateTime</span></span>|<span data-ttu-id="33f93-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33f93-158">DateTimeOffset</span></span>|<span data-ttu-id="33f93-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-159">The date and time the app was last modified.</span></span> <span data-ttu-id="33f93-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="33f93-161">isFeatured</span></span>|<span data-ttu-id="33f93-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="33f93-162">Boolean</span></span>|<span data-ttu-id="33f93-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="33f93-164">privacyInformationUrl</span></span>|<span data-ttu-id="33f93-165">String</span><span class="sxs-lookup"><span data-stu-id="33f93-165">String</span></span>|<span data-ttu-id="33f93-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="33f93-166">The privacy statement Url.</span></span> <span data-ttu-id="33f93-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="33f93-168">informationUrl</span></span>|<span data-ttu-id="33f93-169">String</span><span class="sxs-lookup"><span data-stu-id="33f93-169">String</span></span>|<span data-ttu-id="33f93-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="33f93-170">The more information Url.</span></span> <span data-ttu-id="33f93-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-172">owner</span><span class="sxs-lookup"><span data-stu-id="33f93-172">owner</span></span>|<span data-ttu-id="33f93-173">String</span><span class="sxs-lookup"><span data-stu-id="33f93-173">String</span></span>|<span data-ttu-id="33f93-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-174">The owner of the app.</span></span> <span data-ttu-id="33f93-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-176">developer</span><span class="sxs-lookup"><span data-stu-id="33f93-176">developer</span></span>|<span data-ttu-id="33f93-177">String</span><span class="sxs-lookup"><span data-stu-id="33f93-177">String</span></span>|<span data-ttu-id="33f93-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-178">The developer of the app.</span></span> <span data-ttu-id="33f93-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-180">notes</span><span class="sxs-lookup"><span data-stu-id="33f93-180">notes</span></span>|<span data-ttu-id="33f93-181">String</span><span class="sxs-lookup"><span data-stu-id="33f93-181">String</span></span>|<span data-ttu-id="33f93-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-182">Notes for the app.</span></span> <span data-ttu-id="33f93-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="33f93-184">uploadState</span></span>|<span data-ttu-id="33f93-185">Int32</span><span class="sxs-lookup"><span data-stu-id="33f93-185">Int32</span></span>|<span data-ttu-id="33f93-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="33f93-186">The upload state.</span></span> <span data-ttu-id="33f93-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="33f93-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="33f93-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="33f93-189">publishingState</span></span>|[<span data-ttu-id="33f93-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="33f93-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="33f93-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-191">The publishing state for the app.</span></span> <span data-ttu-id="33f93-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="33f93-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="33f93-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="33f93-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="33f93-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="33f93-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="33f93-195">isAssigned</span></span>|<span data-ttu-id="33f93-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="33f93-196">Boolean</span></span>|<span data-ttu-id="33f93-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="33f93-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="33f93-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33f93-199">roleScopeTagIds</span></span>|<span data-ttu-id="33f93-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33f93-200">String collection</span></span>|<span data-ttu-id="33f93-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="33f93-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="33f93-203">dependentAppCount</span></span>|<span data-ttu-id="33f93-204">Int32</span><span class="sxs-lookup"><span data-stu-id="33f93-204">Int32</span></span>|<span data-ttu-id="33f93-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="33f93-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="33f93-207">supersedingAppCount</span></span>|<span data-ttu-id="33f93-208">Int32</span><span class="sxs-lookup"><span data-stu-id="33f93-208">Int32</span></span>|<span data-ttu-id="33f93-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="33f93-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="33f93-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="33f93-211">supersededAppCount</span></span>|<span data-ttu-id="33f93-212">Int32</span><span class="sxs-lookup"><span data-stu-id="33f93-212">Int32</span></span>|<span data-ttu-id="33f93-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="33f93-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="33f93-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33f93-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="33f93-215">committedContentVersion</span></span>|<span data-ttu-id="33f93-216">String</span><span class="sxs-lookup"><span data-stu-id="33f93-216">String</span></span>|<span data-ttu-id="33f93-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="33f93-217">The internal committed content version.</span></span> <span data-ttu-id="33f93-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="33f93-219">fileName</span><span class="sxs-lookup"><span data-stu-id="33f93-219">fileName</span></span>|<span data-ttu-id="33f93-220">String</span><span class="sxs-lookup"><span data-stu-id="33f93-220">String</span></span>|<span data-ttu-id="33f93-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="33f93-221">The name of the main Lob application file.</span></span> <span data-ttu-id="33f93-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="33f93-223">size</span><span class="sxs-lookup"><span data-stu-id="33f93-223">size</span></span>|<span data-ttu-id="33f93-224">Int64</span><span class="sxs-lookup"><span data-stu-id="33f93-224">Int64</span></span>|<span data-ttu-id="33f93-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="33f93-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="33f93-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="33f93-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="33f93-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="33f93-227">applicableArchitectures</span></span>|[<span data-ttu-id="33f93-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="33f93-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="33f93-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="33f93-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="33f93-230">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="33f93-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="33f93-231">identityName</span><span class="sxs-lookup"><span data-stu-id="33f93-231">identityName</span></span>|<span data-ttu-id="33f93-232">String</span><span class="sxs-lookup"><span data-stu-id="33f93-232">String</span></span>|<span data-ttu-id="33f93-233">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="33f93-233">The Identity Name.</span></span>|
|<span data-ttu-id="33f93-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="33f93-234">identityPublisherHash</span></span>|<span data-ttu-id="33f93-235">String</span><span class="sxs-lookup"><span data-stu-id="33f93-235">String</span></span>|<span data-ttu-id="33f93-236">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="33f93-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="33f93-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="33f93-237">identityResourceIdentifier</span></span>|<span data-ttu-id="33f93-238">String</span><span class="sxs-lookup"><span data-stu-id="33f93-238">String</span></span>|<span data-ttu-id="33f93-239">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="33f93-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="33f93-240">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="33f93-240">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="33f93-241">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="33f93-241">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="33f93-242">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="33f93-242">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="33f93-243">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="33f93-243">phoneProductIdentifier</span></span>|<span data-ttu-id="33f93-244">Строка</span><span class="sxs-lookup"><span data-stu-id="33f93-244">String</span></span>|<span data-ttu-id="33f93-245">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="33f93-245">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="33f93-246">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="33f93-246">phonePublisherId</span></span>|<span data-ttu-id="33f93-247">Строка</span><span class="sxs-lookup"><span data-stu-id="33f93-247">String</span></span>|<span data-ttu-id="33f93-248">Идентификатор издателя телефона.</span><span class="sxs-lookup"><span data-stu-id="33f93-248">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="33f93-249">identityVersion</span><span class="sxs-lookup"><span data-stu-id="33f93-249">identityVersion</span></span>|<span data-ttu-id="33f93-250">String</span><span class="sxs-lookup"><span data-stu-id="33f93-250">String</span></span>|<span data-ttu-id="33f93-251">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="33f93-251">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="33f93-252">Ответ</span><span class="sxs-lookup"><span data-stu-id="33f93-252">Response</span></span>
<span data-ttu-id="33f93-253">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33f93-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f93-254">Пример</span><span class="sxs-lookup"><span data-stu-id="33f93-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="33f93-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="33f93-255">Request</span></span>
<span data-ttu-id="33f93-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33f93-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1570

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="33f93-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="33f93-257">Response</span></span>
<span data-ttu-id="33f93-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33f93-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1742

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```





