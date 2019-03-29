---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80b00bf14177b64db028ad6a32a0a45338dd93db
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968765"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="f3463-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="f3463-103">Create androidStoreApp</span></span>

> <span data-ttu-id="f3463-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3463-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3463-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3463-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3463-106">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3463-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f3463-107">Prerequisites</span></span>
<span data-ttu-id="f3463-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3463-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3463-110">Permission type</span></span>|<span data-ttu-id="f3463-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3463-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3463-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3463-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3463-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3463-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3463-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3463-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3463-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3463-115">Not supported.</span></span>|
|<span data-ttu-id="f3463-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3463-116">Application</span></span>|<span data-ttu-id="f3463-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3463-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3463-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3463-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f3463-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3463-119">Request headers</span></span>
|<span data-ttu-id="f3463-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3463-120">Header</span></span>|<span data-ttu-id="f3463-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f3463-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3463-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3463-122">Authorization</span></span>|<span data-ttu-id="f3463-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3463-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3463-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f3463-124">Accept</span></span>|<span data-ttu-id="f3463-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3463-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3463-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3463-126">Request body</span></span>
<span data-ttu-id="f3463-127">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3463-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="f3463-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="f3463-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="f3463-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3463-129">Property</span></span>|<span data-ttu-id="f3463-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f3463-130">Type</span></span>|<span data-ttu-id="f3463-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f3463-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3463-132">id</span><span class="sxs-lookup"><span data-stu-id="f3463-132">id</span></span>|<span data-ttu-id="f3463-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f3463-133">String</span></span>|<span data-ttu-id="f3463-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3463-134">Key of the entity.</span></span> <span data-ttu-id="f3463-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f3463-136">displayName</span></span>|<span data-ttu-id="f3463-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f3463-137">String</span></span>|<span data-ttu-id="f3463-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f3463-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f3463-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-140">description</span><span class="sxs-lookup"><span data-stu-id="f3463-140">description</span></span>|<span data-ttu-id="f3463-141">String</span><span class="sxs-lookup"><span data-stu-id="f3463-141">String</span></span>|<span data-ttu-id="f3463-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-142">The description of the app.</span></span> <span data-ttu-id="f3463-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f3463-144">publisher</span></span>|<span data-ttu-id="f3463-145">String</span><span class="sxs-lookup"><span data-stu-id="f3463-145">String</span></span>|<span data-ttu-id="f3463-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-146">The publisher of the app.</span></span> <span data-ttu-id="f3463-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f3463-148">largeIcon</span></span>|[<span data-ttu-id="f3463-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3463-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3463-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f3463-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f3463-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3463-152">createdDateTime</span></span>|<span data-ttu-id="f3463-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3463-153">DateTimeOffset</span></span>|<span data-ttu-id="f3463-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-154">The date and time the app was created.</span></span> <span data-ttu-id="f3463-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3463-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f3463-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3463-157">DateTimeOffset</span></span>|<span data-ttu-id="f3463-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f3463-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f3463-160">isFeatured</span></span>|<span data-ttu-id="f3463-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3463-161">Boolean</span></span>|<span data-ttu-id="f3463-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3463-163">privacyInformationUrl</span></span>|<span data-ttu-id="f3463-164">String</span><span class="sxs-lookup"><span data-stu-id="f3463-164">String</span></span>|<span data-ttu-id="f3463-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f3463-165">The privacy statement Url.</span></span> <span data-ttu-id="f3463-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3463-167">informationUrl</span></span>|<span data-ttu-id="f3463-168">String</span><span class="sxs-lookup"><span data-stu-id="f3463-168">String</span></span>|<span data-ttu-id="f3463-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f3463-169">The more information Url.</span></span> <span data-ttu-id="f3463-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-171">owner</span><span class="sxs-lookup"><span data-stu-id="f3463-171">owner</span></span>|<span data-ttu-id="f3463-172">String</span><span class="sxs-lookup"><span data-stu-id="f3463-172">String</span></span>|<span data-ttu-id="f3463-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-173">The owner of the app.</span></span> <span data-ttu-id="f3463-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-175">developer</span><span class="sxs-lookup"><span data-stu-id="f3463-175">developer</span></span>|<span data-ttu-id="f3463-176">String</span><span class="sxs-lookup"><span data-stu-id="f3463-176">String</span></span>|<span data-ttu-id="f3463-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-177">The developer of the app.</span></span> <span data-ttu-id="f3463-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-179">notes</span><span class="sxs-lookup"><span data-stu-id="f3463-179">notes</span></span>|<span data-ttu-id="f3463-180">String</span><span class="sxs-lookup"><span data-stu-id="f3463-180">String</span></span>|<span data-ttu-id="f3463-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-181">Notes for the app.</span></span> <span data-ttu-id="f3463-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f3463-183">uploadState</span></span>|<span data-ttu-id="f3463-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f3463-184">Int32</span></span>|<span data-ttu-id="f3463-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="f3463-185">The upload state.</span></span> <span data-ttu-id="f3463-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f3463-187">publishingState</span></span>|[<span data-ttu-id="f3463-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f3463-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f3463-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-189">The publishing state for the app.</span></span> <span data-ttu-id="f3463-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f3463-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f3463-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f3463-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f3463-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f3463-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f3463-193">isAssigned</span></span>|<span data-ttu-id="f3463-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3463-194">Boolean</span></span>|<span data-ttu-id="f3463-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="f3463-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f3463-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3463-197">roleScopeTagIds</span></span>|<span data-ttu-id="f3463-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f3463-198">String collection</span></span>|<span data-ttu-id="f3463-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f3463-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f3463-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3463-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3463-201">packageId</span><span class="sxs-lookup"><span data-stu-id="f3463-201">packageId</span></span>|<span data-ttu-id="f3463-202">String</span><span class="sxs-lookup"><span data-stu-id="f3463-202">String</span></span>|<span data-ttu-id="f3463-203">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="f3463-203">The package identifier.</span></span>|
|<span data-ttu-id="f3463-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3463-204">appIdentifier</span></span>|<span data-ttu-id="f3463-205">String</span><span class="sxs-lookup"><span data-stu-id="f3463-205">String</span></span>|<span data-ttu-id="f3463-206">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f3463-206">The Identity Name.</span></span>|
|<span data-ttu-id="f3463-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f3463-207">appStoreUrl</span></span>|<span data-ttu-id="f3463-208">String</span><span class="sxs-lookup"><span data-stu-id="f3463-208">String</span></span>|<span data-ttu-id="f3463-209">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="f3463-209">The Android app store URL.</span></span>|
|<span data-ttu-id="f3463-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3463-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f3463-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3463-211">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f3463-212">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f3463-212">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f3463-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3463-213">Response</span></span>
<span data-ttu-id="f3463-214">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3463-214">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3463-215">Пример</span><span class="sxs-lookup"><span data-stu-id="f3463-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3463-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3463-216">Request</span></span>
<span data-ttu-id="f3463-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3463-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1203

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="f3463-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3463-218">Response</span></span>
<span data-ttu-id="f3463-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3463-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1375

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```




