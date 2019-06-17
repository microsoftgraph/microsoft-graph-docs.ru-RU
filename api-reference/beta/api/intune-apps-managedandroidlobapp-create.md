---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe1907a05707ec5f6e4903c84c4134697adc2e88
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975086"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="e5c96-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="e5c96-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="e5c96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5c96-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5c96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5c96-106">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-106">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5c96-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c96-107">Prerequisites</span></span>
<span data-ttu-id="e5c96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c96-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c96-110">Permission type</span></span>|<span data-ttu-id="e5c96-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5c96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5c96-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5c96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5c96-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c96-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5c96-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5c96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5c96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c96-115">Not supported.</span></span>|
|<span data-ttu-id="e5c96-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5c96-116">Application</span></span>|<span data-ttu-id="e5c96-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c96-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5c96-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5c96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e5c96-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5c96-119">Request headers</span></span>
|<span data-ttu-id="e5c96-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5c96-120">Header</span></span>|<span data-ttu-id="e5c96-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5c96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5c96-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5c96-122">Authorization</span></span>|<span data-ttu-id="e5c96-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5c96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5c96-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5c96-124">Accept</span></span>|<span data-ttu-id="e5c96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5c96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5c96-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5c96-126">Request body</span></span>
<span data-ttu-id="e5c96-127">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5c96-127">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="e5c96-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="e5c96-128">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="e5c96-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5c96-129">Property</span></span>|<span data-ttu-id="e5c96-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5c96-130">Type</span></span>|<span data-ttu-id="e5c96-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5c96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5c96-132">id</span><span class="sxs-lookup"><span data-stu-id="e5c96-132">id</span></span>|<span data-ttu-id="e5c96-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e5c96-133">String</span></span>|<span data-ttu-id="e5c96-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5c96-134">Key of the entity.</span></span> <span data-ttu-id="e5c96-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e5c96-136">displayName</span></span>|<span data-ttu-id="e5c96-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e5c96-137">String</span></span>|<span data-ttu-id="e5c96-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e5c96-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e5c96-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-140">description</span><span class="sxs-lookup"><span data-stu-id="e5c96-140">description</span></span>|<span data-ttu-id="e5c96-141">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-141">String</span></span>|<span data-ttu-id="e5c96-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-142">The description of the app.</span></span> <span data-ttu-id="e5c96-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e5c96-144">publisher</span></span>|<span data-ttu-id="e5c96-145">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-145">String</span></span>|<span data-ttu-id="e5c96-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-146">The publisher of the app.</span></span> <span data-ttu-id="e5c96-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e5c96-148">largeIcon</span></span>|[<span data-ttu-id="e5c96-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e5c96-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e5c96-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e5c96-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e5c96-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5c96-152">createdDateTime</span></span>|<span data-ttu-id="e5c96-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5c96-153">DateTimeOffset</span></span>|<span data-ttu-id="e5c96-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-154">The date and time the app was created.</span></span> <span data-ttu-id="e5c96-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5c96-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e5c96-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5c96-157">DateTimeOffset</span></span>|<span data-ttu-id="e5c96-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e5c96-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e5c96-160">isFeatured</span></span>|<span data-ttu-id="e5c96-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5c96-161">Boolean</span></span>|<span data-ttu-id="e5c96-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e5c96-163">privacyInformationUrl</span></span>|<span data-ttu-id="e5c96-164">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-164">String</span></span>|<span data-ttu-id="e5c96-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e5c96-165">The privacy statement Url.</span></span> <span data-ttu-id="e5c96-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e5c96-167">informationUrl</span></span>|<span data-ttu-id="e5c96-168">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-168">String</span></span>|<span data-ttu-id="e5c96-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e5c96-169">The more information Url.</span></span> <span data-ttu-id="e5c96-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-171">owner</span><span class="sxs-lookup"><span data-stu-id="e5c96-171">owner</span></span>|<span data-ttu-id="e5c96-172">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-172">String</span></span>|<span data-ttu-id="e5c96-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-173">The owner of the app.</span></span> <span data-ttu-id="e5c96-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-175">developer</span><span class="sxs-lookup"><span data-stu-id="e5c96-175">developer</span></span>|<span data-ttu-id="e5c96-176">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-176">String</span></span>|<span data-ttu-id="e5c96-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-177">The developer of the app.</span></span> <span data-ttu-id="e5c96-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-179">notes</span><span class="sxs-lookup"><span data-stu-id="e5c96-179">notes</span></span>|<span data-ttu-id="e5c96-180">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-180">String</span></span>|<span data-ttu-id="e5c96-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-181">Notes for the app.</span></span> <span data-ttu-id="e5c96-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e5c96-183">uploadState</span></span>|<span data-ttu-id="e5c96-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e5c96-184">Int32</span></span>|<span data-ttu-id="e5c96-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="e5c96-185">The upload state.</span></span> <span data-ttu-id="e5c96-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e5c96-187">publishingState</span></span>|[<span data-ttu-id="e5c96-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="e5c96-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e5c96-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-189">The publishing state for the app.</span></span> <span data-ttu-id="e5c96-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e5c96-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e5c96-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e5c96-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e5c96-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e5c96-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e5c96-193">isAssigned</span></span>|<span data-ttu-id="e5c96-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5c96-194">Boolean</span></span>|<span data-ttu-id="e5c96-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="e5c96-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e5c96-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5c96-197">roleScopeTagIds</span></span>|<span data-ttu-id="e5c96-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e5c96-198">String collection</span></span>|<span data-ttu-id="e5c96-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e5c96-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="e5c96-201">dependentAppCount</span></span>|<span data-ttu-id="e5c96-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e5c96-202">Int32</span></span>|<span data-ttu-id="e5c96-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e5c96-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5c96-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e5c96-205">appAvailability</span></span>|[<span data-ttu-id="e5c96-206">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="e5c96-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e5c96-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-207">The Application's availability.</span></span> <span data-ttu-id="e5c96-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e5c96-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e5c96-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e5c96-210">version</span><span class="sxs-lookup"><span data-stu-id="e5c96-210">version</span></span>|<span data-ttu-id="e5c96-211">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-211">String</span></span>|<span data-ttu-id="e5c96-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-212">The Application's version.</span></span> <span data-ttu-id="e5c96-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e5c96-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e5c96-214">committedContentVersion</span></span>|<span data-ttu-id="e5c96-215">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-215">String</span></span>|<span data-ttu-id="e5c96-216">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e5c96-216">The internal committed content version.</span></span> <span data-ttu-id="e5c96-217">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e5c96-218">fileName</span><span class="sxs-lookup"><span data-stu-id="e5c96-218">fileName</span></span>|<span data-ttu-id="e5c96-219">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-219">String</span></span>|<span data-ttu-id="e5c96-220">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-220">The name of the main Lob application file.</span></span> <span data-ttu-id="e5c96-221">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e5c96-222">size</span><span class="sxs-lookup"><span data-stu-id="e5c96-222">size</span></span>|<span data-ttu-id="e5c96-223">Int64</span><span class="sxs-lookup"><span data-stu-id="e5c96-223">Int64</span></span>|<span data-ttu-id="e5c96-224">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e5c96-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="e5c96-225">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5c96-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e5c96-226">packageId</span><span class="sxs-lookup"><span data-stu-id="e5c96-226">packageId</span></span>|<span data-ttu-id="e5c96-227">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-227">String</span></span>|<span data-ttu-id="e5c96-228">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="e5c96-228">The package identifier.</span></span>|
|<span data-ttu-id="e5c96-229">identityName</span><span class="sxs-lookup"><span data-stu-id="e5c96-229">identityName</span></span>|<span data-ttu-id="e5c96-230">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-230">String</span></span>|<span data-ttu-id="e5c96-231">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-231">The Identity Name.</span></span>|
|<span data-ttu-id="e5c96-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e5c96-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e5c96-233">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e5c96-233">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e5c96-234">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e5c96-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e5c96-235">versionName</span><span class="sxs-lookup"><span data-stu-id="e5c96-235">versionName</span></span>|<span data-ttu-id="e5c96-236">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-236">String</span></span>|<span data-ttu-id="e5c96-237">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="e5c96-237">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e5c96-238">versionCode</span><span class="sxs-lookup"><span data-stu-id="e5c96-238">versionCode</span></span>|<span data-ttu-id="e5c96-239">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-239">String</span></span>|<span data-ttu-id="e5c96-240">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="e5c96-240">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e5c96-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e5c96-241">identityVersion</span></span>|<span data-ttu-id="e5c96-242">String</span><span class="sxs-lookup"><span data-stu-id="e5c96-242">String</span></span>|<span data-ttu-id="e5c96-243">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e5c96-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e5c96-244">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5c96-244">Response</span></span>
<span data-ttu-id="e5c96-245">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e5c96-245">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5c96-246">Пример</span><span class="sxs-lookup"><span data-stu-id="e5c96-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5c96-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5c96-247">Request</span></span>
<span data-ttu-id="e5c96-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5c96-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1491

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e5c96-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5c96-249">Response</span></span>
<span data-ttu-id="e5c96-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5c96-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1663

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





