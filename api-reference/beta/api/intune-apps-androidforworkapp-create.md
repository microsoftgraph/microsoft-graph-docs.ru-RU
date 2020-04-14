---
title: Создание Андроидфорворкапп
description: Создание нового объекта Андроидфорворкапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57282cd5287b89d623fcf13bf646df6bd19f7a57
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417828"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="d7d92-103">Создание Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="d7d92-103">Create androidForWorkApp</span></span>

<span data-ttu-id="d7d92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7d92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7d92-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7d92-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7d92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7d92-107">Создание нового объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d7d92-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7d92-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7d92-108">Prerequisites</span></span>
<span data-ttu-id="d7d92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7d92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7d92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d92-111">Permission type</span></span>|<span data-ttu-id="d7d92-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7d92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7d92-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7d92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7d92-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7d92-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7d92-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7d92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7d92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d92-116">Not supported.</span></span>|
|<span data-ttu-id="d7d92-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7d92-117">Application</span></span>|<span data-ttu-id="d7d92-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7d92-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7d92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7d92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d7d92-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7d92-120">Request headers</span></span>
|<span data-ttu-id="d7d92-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7d92-121">Header</span></span>|<span data-ttu-id="d7d92-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7d92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7d92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7d92-123">Authorization</span></span>|<span data-ttu-id="d7d92-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7d92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7d92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7d92-125">Accept</span></span>|<span data-ttu-id="d7d92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7d92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7d92-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7d92-127">Request body</span></span>
<span data-ttu-id="d7d92-128">В тексте запроса добавьте представление объекта Андроидфорворкапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7d92-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="d7d92-129">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкапп.</span><span class="sxs-lookup"><span data-stu-id="d7d92-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="d7d92-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7d92-130">Property</span></span>|<span data-ttu-id="d7d92-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d92-131">Type</span></span>|<span data-ttu-id="d7d92-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7d92-133">id</span><span class="sxs-lookup"><span data-stu-id="d7d92-133">id</span></span>|<span data-ttu-id="d7d92-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d92-134">String</span></span>|<span data-ttu-id="d7d92-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7d92-135">Key of the entity.</span></span> <span data-ttu-id="d7d92-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d7d92-137">displayName</span></span>|<span data-ttu-id="d7d92-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d92-138">String</span></span>|<span data-ttu-id="d7d92-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d7d92-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d7d92-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-141">description</span><span class="sxs-lookup"><span data-stu-id="d7d92-141">description</span></span>|<span data-ttu-id="d7d92-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d92-142">String</span></span>|<span data-ttu-id="d7d92-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-143">The description of the app.</span></span> <span data-ttu-id="d7d92-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d7d92-145">publisher</span></span>|<span data-ttu-id="d7d92-146">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-146">String</span></span>|<span data-ttu-id="d7d92-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-147">The publisher of the app.</span></span> <span data-ttu-id="d7d92-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d7d92-149">largeIcon</span></span>|[<span data-ttu-id="d7d92-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d7d92-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d7d92-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d7d92-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d7d92-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d92-153">createdDateTime</span></span>|<span data-ttu-id="d7d92-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d92-154">DateTimeOffset</span></span>|<span data-ttu-id="d7d92-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-155">The date and time the app was created.</span></span> <span data-ttu-id="d7d92-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d92-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d7d92-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d92-158">DateTimeOffset</span></span>|<span data-ttu-id="d7d92-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d7d92-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d7d92-161">isFeatured</span></span>|<span data-ttu-id="d7d92-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7d92-162">Boolean</span></span>|<span data-ttu-id="d7d92-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d7d92-164">privacyInformationUrl</span></span>|<span data-ttu-id="d7d92-165">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-165">String</span></span>|<span data-ttu-id="d7d92-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d7d92-166">The privacy statement Url.</span></span> <span data-ttu-id="d7d92-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d7d92-168">informationUrl</span></span>|<span data-ttu-id="d7d92-169">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-169">String</span></span>|<span data-ttu-id="d7d92-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d7d92-170">The more information Url.</span></span> <span data-ttu-id="d7d92-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-172">owner</span><span class="sxs-lookup"><span data-stu-id="d7d92-172">owner</span></span>|<span data-ttu-id="d7d92-173">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-173">String</span></span>|<span data-ttu-id="d7d92-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-174">The owner of the app.</span></span> <span data-ttu-id="d7d92-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-176">developer</span><span class="sxs-lookup"><span data-stu-id="d7d92-176">developer</span></span>|<span data-ttu-id="d7d92-177">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-177">String</span></span>|<span data-ttu-id="d7d92-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-178">The developer of the app.</span></span> <span data-ttu-id="d7d92-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-180">notes</span><span class="sxs-lookup"><span data-stu-id="d7d92-180">notes</span></span>|<span data-ttu-id="d7d92-181">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-181">String</span></span>|<span data-ttu-id="d7d92-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-182">Notes for the app.</span></span> <span data-ttu-id="d7d92-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d7d92-184">uploadState</span></span>|<span data-ttu-id="d7d92-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d92-185">Int32</span></span>|<span data-ttu-id="d7d92-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="d7d92-186">The upload state.</span></span> <span data-ttu-id="d7d92-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d7d92-188">publishingState</span></span>|[<span data-ttu-id="d7d92-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d7d92-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d7d92-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-190">The publishing state for the app.</span></span> <span data-ttu-id="d7d92-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d7d92-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d7d92-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d7d92-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d7d92-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d7d92-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d7d92-194">isAssigned</span></span>|<span data-ttu-id="d7d92-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7d92-195">Boolean</span></span>|<span data-ttu-id="d7d92-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="d7d92-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d7d92-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7d92-198">roleScopeTagIds</span></span>|<span data-ttu-id="d7d92-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d7d92-199">String collection</span></span>|<span data-ttu-id="d7d92-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d7d92-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="d7d92-202">dependentAppCount</span></span>|<span data-ttu-id="d7d92-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d92-203">Int32</span></span>|<span data-ttu-id="d7d92-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d7d92-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d92-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d92-206">packageId</span><span class="sxs-lookup"><span data-stu-id="d7d92-206">packageId</span></span>|<span data-ttu-id="d7d92-207">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-207">String</span></span>|<span data-ttu-id="d7d92-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="d7d92-208">The package identifier.</span></span>|
|<span data-ttu-id="d7d92-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7d92-209">appIdentifier</span></span>|<span data-ttu-id="d7d92-210">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-210">String</span></span>|<span data-ttu-id="d7d92-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d7d92-211">The Identity Name.</span></span>|
|<span data-ttu-id="d7d92-212">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d7d92-212">usedLicenseCount</span></span>|<span data-ttu-id="d7d92-213">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d92-213">Int32</span></span>|<span data-ttu-id="d7d92-214">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d7d92-214">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="d7d92-215">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d7d92-215">totalLicenseCount</span></span>|<span data-ttu-id="d7d92-216">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d92-216">Int32</span></span>|<span data-ttu-id="d7d92-217">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d7d92-217">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="d7d92-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d7d92-218">appStoreUrl</span></span>|<span data-ttu-id="d7d92-219">String</span><span class="sxs-lookup"><span data-stu-id="d7d92-219">String</span></span>|<span data-ttu-id="d7d92-220">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="d7d92-220">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="d7d92-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d92-221">Response</span></span>
<span data-ttu-id="d7d92-222">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7d92-222">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7d92-223">Пример</span><span class="sxs-lookup"><span data-stu-id="d7d92-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7d92-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7d92-224">Request</span></span>
<span data-ttu-id="d7d92-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7d92-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 903

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="d7d92-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d92-226">Response</span></span>
<span data-ttu-id="d7d92-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7d92-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1075

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```



