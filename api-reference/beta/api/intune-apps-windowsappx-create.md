---
title: Создание windowsAppX
description: Создание нового объекта windowsAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1472de7e4db226570e599072f541a3e1884de2a6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961254"
---
# <a name="create-windowsappx"></a><span data-ttu-id="0f966-103">Создание windowsAppX</span><span class="sxs-lookup"><span data-stu-id="0f966-103">Create windowsAppX</span></span>

> <span data-ttu-id="0f966-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f966-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f966-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f966-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f966-106">Создание нового объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="0f966-106">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f966-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0f966-107">Prerequisites</span></span>
<span data-ttu-id="0f966-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f966-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f966-110">Permission type</span></span>|<span data-ttu-id="0f966-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f966-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f966-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f966-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f966-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f966-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f966-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f966-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f966-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f966-115">Not supported.</span></span>|
|<span data-ttu-id="0f966-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f966-116">Application</span></span>|<span data-ttu-id="0f966-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f966-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f966-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f966-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0f966-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f966-119">Request headers</span></span>
|<span data-ttu-id="0f966-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f966-120">Header</span></span>|<span data-ttu-id="0f966-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0f966-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f966-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f966-122">Authorization</span></span>|<span data-ttu-id="0f966-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f966-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f966-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0f966-124">Accept</span></span>|<span data-ttu-id="0f966-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f966-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f966-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f966-126">Request body</span></span>
<span data-ttu-id="0f966-127">В тексте запроса добавьте представление объекта windowsAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f966-127">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="0f966-128">В следующей таблице приведены свойства, необходимые при создании windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="0f966-128">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="0f966-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f966-129">Property</span></span>|<span data-ttu-id="0f966-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0f966-130">Type</span></span>|<span data-ttu-id="0f966-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0f966-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f966-132">id</span><span class="sxs-lookup"><span data-stu-id="0f966-132">id</span></span>|<span data-ttu-id="0f966-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0f966-133">String</span></span>|<span data-ttu-id="0f966-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f966-134">Key of the entity.</span></span> <span data-ttu-id="0f966-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0f966-136">displayName</span></span>|<span data-ttu-id="0f966-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0f966-137">String</span></span>|<span data-ttu-id="0f966-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0f966-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0f966-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-140">description</span><span class="sxs-lookup"><span data-stu-id="0f966-140">description</span></span>|<span data-ttu-id="0f966-141">String</span><span class="sxs-lookup"><span data-stu-id="0f966-141">String</span></span>|<span data-ttu-id="0f966-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-142">The description of the app.</span></span> <span data-ttu-id="0f966-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0f966-144">publisher</span></span>|<span data-ttu-id="0f966-145">String</span><span class="sxs-lookup"><span data-stu-id="0f966-145">String</span></span>|<span data-ttu-id="0f966-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-146">The publisher of the app.</span></span> <span data-ttu-id="0f966-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0f966-148">largeIcon</span></span>|[<span data-ttu-id="0f966-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f966-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f966-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0f966-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0f966-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f966-152">createdDateTime</span></span>|<span data-ttu-id="0f966-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f966-153">DateTimeOffset</span></span>|<span data-ttu-id="0f966-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-154">The date and time the app was created.</span></span> <span data-ttu-id="0f966-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f966-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0f966-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f966-157">DateTimeOffset</span></span>|<span data-ttu-id="0f966-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0f966-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0f966-160">isFeatured</span></span>|<span data-ttu-id="0f966-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f966-161">Boolean</span></span>|<span data-ttu-id="0f966-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f966-163">privacyInformationUrl</span></span>|<span data-ttu-id="0f966-164">String</span><span class="sxs-lookup"><span data-stu-id="0f966-164">String</span></span>|<span data-ttu-id="0f966-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0f966-165">The privacy statement Url.</span></span> <span data-ttu-id="0f966-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f966-167">informationUrl</span></span>|<span data-ttu-id="0f966-168">String</span><span class="sxs-lookup"><span data-stu-id="0f966-168">String</span></span>|<span data-ttu-id="0f966-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0f966-169">The more information Url.</span></span> <span data-ttu-id="0f966-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-171">owner</span><span class="sxs-lookup"><span data-stu-id="0f966-171">owner</span></span>|<span data-ttu-id="0f966-172">String</span><span class="sxs-lookup"><span data-stu-id="0f966-172">String</span></span>|<span data-ttu-id="0f966-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-173">The owner of the app.</span></span> <span data-ttu-id="0f966-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-175">developer</span><span class="sxs-lookup"><span data-stu-id="0f966-175">developer</span></span>|<span data-ttu-id="0f966-176">String</span><span class="sxs-lookup"><span data-stu-id="0f966-176">String</span></span>|<span data-ttu-id="0f966-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-177">The developer of the app.</span></span> <span data-ttu-id="0f966-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-179">notes</span><span class="sxs-lookup"><span data-stu-id="0f966-179">notes</span></span>|<span data-ttu-id="0f966-180">String</span><span class="sxs-lookup"><span data-stu-id="0f966-180">String</span></span>|<span data-ttu-id="0f966-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-181">Notes for the app.</span></span> <span data-ttu-id="0f966-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0f966-183">uploadState</span></span>|<span data-ttu-id="0f966-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0f966-184">Int32</span></span>|<span data-ttu-id="0f966-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="0f966-185">The upload state.</span></span> <span data-ttu-id="0f966-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0f966-187">publishingState</span></span>|[<span data-ttu-id="0f966-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="0f966-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0f966-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-189">The publishing state for the app.</span></span> <span data-ttu-id="0f966-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0f966-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0f966-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0f966-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0f966-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0f966-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0f966-193">isAssigned</span></span>|<span data-ttu-id="0f966-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f966-194">Boolean</span></span>|<span data-ttu-id="0f966-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="0f966-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0f966-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f966-197">roleScopeTagIds</span></span>|<span data-ttu-id="0f966-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0f966-198">String collection</span></span>|<span data-ttu-id="0f966-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0f966-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f966-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0f966-201">committedContentVersion</span></span>|<span data-ttu-id="0f966-202">String</span><span class="sxs-lookup"><span data-stu-id="0f966-202">String</span></span>|<span data-ttu-id="0f966-203">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="0f966-203">The internal committed content version.</span></span> <span data-ttu-id="0f966-204">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0f966-205">fileName</span><span class="sxs-lookup"><span data-stu-id="0f966-205">fileName</span></span>|<span data-ttu-id="0f966-206">String</span><span class="sxs-lookup"><span data-stu-id="0f966-206">String</span></span>|<span data-ttu-id="0f966-207">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="0f966-207">The name of the main Lob application file.</span></span> <span data-ttu-id="0f966-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0f966-209">size</span><span class="sxs-lookup"><span data-stu-id="0f966-209">size</span></span>|<span data-ttu-id="0f966-210">Int64</span><span class="sxs-lookup"><span data-stu-id="0f966-210">Int64</span></span>|<span data-ttu-id="0f966-211">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="0f966-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="0f966-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f966-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0f966-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="0f966-213">applicableArchitectures</span></span>|[<span data-ttu-id="0f966-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0f966-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0f966-215">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="0f966-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="0f966-216">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="0f966-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="0f966-217">identityName</span><span class="sxs-lookup"><span data-stu-id="0f966-217">identityName</span></span>|<span data-ttu-id="0f966-218">String</span><span class="sxs-lookup"><span data-stu-id="0f966-218">String</span></span>|<span data-ttu-id="0f966-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0f966-219">The Identity Name.</span></span>|
|<span data-ttu-id="0f966-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="0f966-220">identityPublisherHash</span></span>|<span data-ttu-id="0f966-221">String</span><span class="sxs-lookup"><span data-stu-id="0f966-221">String</span></span>|<span data-ttu-id="0f966-222">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="0f966-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="0f966-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0f966-223">identityResourceIdentifier</span></span>|<span data-ttu-id="0f966-224">String</span><span class="sxs-lookup"><span data-stu-id="0f966-224">String</span></span>|<span data-ttu-id="0f966-225">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="0f966-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="0f966-226">isBundle</span><span class="sxs-lookup"><span data-stu-id="0f966-226">isBundle</span></span>|<span data-ttu-id="0f966-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f966-227">Boolean</span></span>|<span data-ttu-id="0f966-228">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="0f966-228">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="0f966-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f966-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0f966-230">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f966-230">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="0f966-231">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0f966-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0f966-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0f966-232">identityVersion</span></span>|<span data-ttu-id="0f966-233">String</span><span class="sxs-lookup"><span data-stu-id="0f966-233">String</span></span>|<span data-ttu-id="0f966-234">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0f966-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="0f966-235">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f966-235">Response</span></span>
<span data-ttu-id="0f966-236">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAppX](../resources/intune-apps-windowsappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f966-236">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f966-237">Пример</span><span class="sxs-lookup"><span data-stu-id="0f966-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f966-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f966-238">Request</span></span>
<span data-ttu-id="0f966-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f966-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="0f966-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f966-240">Response</span></span>
<span data-ttu-id="0f966-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f966-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1512

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```




