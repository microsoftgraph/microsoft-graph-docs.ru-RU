---
title: Создание windowsPhone81AppX
description: Создание нового объекта windowsPhone81AppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5aa592c91c6680a1b0872c203a10b1a3f4eec55f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983171"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="54f30-103">Создание windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="54f30-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="54f30-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54f30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54f30-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54f30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54f30-106">Создание нового объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="54f30-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54f30-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="54f30-107">Prerequisites</span></span>
<span data-ttu-id="54f30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54f30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54f30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54f30-110">Permission type</span></span>|<span data-ttu-id="54f30-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54f30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54f30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54f30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54f30-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54f30-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54f30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54f30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54f30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54f30-115">Not supported.</span></span>|
|<span data-ttu-id="54f30-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54f30-116">Application</span></span>|<span data-ttu-id="54f30-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54f30-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54f30-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54f30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="54f30-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54f30-119">Request headers</span></span>
|<span data-ttu-id="54f30-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54f30-120">Header</span></span>|<span data-ttu-id="54f30-121">Значение</span><span class="sxs-lookup"><span data-stu-id="54f30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54f30-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54f30-122">Authorization</span></span>|<span data-ttu-id="54f30-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54f30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54f30-124">Accept</span><span class="sxs-lookup"><span data-stu-id="54f30-124">Accept</span></span>|<span data-ttu-id="54f30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54f30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54f30-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54f30-126">Request body</span></span>
<span data-ttu-id="54f30-127">В тексте запроса добавьте представление объекта windowsPhone81AppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54f30-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="54f30-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="54f30-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="54f30-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="54f30-129">Property</span></span>|<span data-ttu-id="54f30-130">Тип</span><span class="sxs-lookup"><span data-stu-id="54f30-130">Type</span></span>|<span data-ttu-id="54f30-131">Описание</span><span class="sxs-lookup"><span data-stu-id="54f30-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54f30-132">id</span><span class="sxs-lookup"><span data-stu-id="54f30-132">id</span></span>|<span data-ttu-id="54f30-133">Строка</span><span class="sxs-lookup"><span data-stu-id="54f30-133">String</span></span>|<span data-ttu-id="54f30-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54f30-134">Key of the entity.</span></span> <span data-ttu-id="54f30-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-136">displayName</span><span class="sxs-lookup"><span data-stu-id="54f30-136">displayName</span></span>|<span data-ttu-id="54f30-137">Строка</span><span class="sxs-lookup"><span data-stu-id="54f30-137">String</span></span>|<span data-ttu-id="54f30-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="54f30-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="54f30-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-140">description</span><span class="sxs-lookup"><span data-stu-id="54f30-140">description</span></span>|<span data-ttu-id="54f30-141">String</span><span class="sxs-lookup"><span data-stu-id="54f30-141">String</span></span>|<span data-ttu-id="54f30-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-142">The description of the app.</span></span> <span data-ttu-id="54f30-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-144">publisher</span><span class="sxs-lookup"><span data-stu-id="54f30-144">publisher</span></span>|<span data-ttu-id="54f30-145">String</span><span class="sxs-lookup"><span data-stu-id="54f30-145">String</span></span>|<span data-ttu-id="54f30-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-146">The publisher of the app.</span></span> <span data-ttu-id="54f30-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="54f30-148">largeIcon</span></span>|[<span data-ttu-id="54f30-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="54f30-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="54f30-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="54f30-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="54f30-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54f30-152">createdDateTime</span></span>|<span data-ttu-id="54f30-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54f30-153">DateTimeOffset</span></span>|<span data-ttu-id="54f30-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-154">The date and time the app was created.</span></span> <span data-ttu-id="54f30-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54f30-156">lastModifiedDateTime</span></span>|<span data-ttu-id="54f30-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54f30-157">DateTimeOffset</span></span>|<span data-ttu-id="54f30-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-158">The date and time the app was last modified.</span></span> <span data-ttu-id="54f30-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="54f30-160">isFeatured</span></span>|<span data-ttu-id="54f30-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="54f30-161">Boolean</span></span>|<span data-ttu-id="54f30-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="54f30-163">privacyInformationUrl</span></span>|<span data-ttu-id="54f30-164">String</span><span class="sxs-lookup"><span data-stu-id="54f30-164">String</span></span>|<span data-ttu-id="54f30-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="54f30-165">The privacy statement Url.</span></span> <span data-ttu-id="54f30-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="54f30-167">informationUrl</span></span>|<span data-ttu-id="54f30-168">String</span><span class="sxs-lookup"><span data-stu-id="54f30-168">String</span></span>|<span data-ttu-id="54f30-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="54f30-169">The more information Url.</span></span> <span data-ttu-id="54f30-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-171">owner</span><span class="sxs-lookup"><span data-stu-id="54f30-171">owner</span></span>|<span data-ttu-id="54f30-172">String</span><span class="sxs-lookup"><span data-stu-id="54f30-172">String</span></span>|<span data-ttu-id="54f30-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-173">The owner of the app.</span></span> <span data-ttu-id="54f30-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-175">developer</span><span class="sxs-lookup"><span data-stu-id="54f30-175">developer</span></span>|<span data-ttu-id="54f30-176">String</span><span class="sxs-lookup"><span data-stu-id="54f30-176">String</span></span>|<span data-ttu-id="54f30-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-177">The developer of the app.</span></span> <span data-ttu-id="54f30-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-179">notes</span><span class="sxs-lookup"><span data-stu-id="54f30-179">notes</span></span>|<span data-ttu-id="54f30-180">String</span><span class="sxs-lookup"><span data-stu-id="54f30-180">String</span></span>|<span data-ttu-id="54f30-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-181">Notes for the app.</span></span> <span data-ttu-id="54f30-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="54f30-183">uploadState</span></span>|<span data-ttu-id="54f30-184">Int32</span><span class="sxs-lookup"><span data-stu-id="54f30-184">Int32</span></span>|<span data-ttu-id="54f30-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="54f30-185">The upload state.</span></span> <span data-ttu-id="54f30-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="54f30-187">publishingState</span></span>|[<span data-ttu-id="54f30-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="54f30-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="54f30-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-189">The publishing state for the app.</span></span> <span data-ttu-id="54f30-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="54f30-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="54f30-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="54f30-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="54f30-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="54f30-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="54f30-193">isAssigned</span></span>|<span data-ttu-id="54f30-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="54f30-194">Boolean</span></span>|<span data-ttu-id="54f30-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="54f30-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="54f30-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54f30-197">roleScopeTagIds</span></span>|<span data-ttu-id="54f30-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="54f30-198">String collection</span></span>|<span data-ttu-id="54f30-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="54f30-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54f30-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="54f30-201">committedContentVersion</span></span>|<span data-ttu-id="54f30-202">String</span><span class="sxs-lookup"><span data-stu-id="54f30-202">String</span></span>|<span data-ttu-id="54f30-203">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="54f30-203">The internal committed content version.</span></span> <span data-ttu-id="54f30-204">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54f30-205">fileName</span><span class="sxs-lookup"><span data-stu-id="54f30-205">fileName</span></span>|<span data-ttu-id="54f30-206">String</span><span class="sxs-lookup"><span data-stu-id="54f30-206">String</span></span>|<span data-ttu-id="54f30-207">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="54f30-207">The name of the main Lob application file.</span></span> <span data-ttu-id="54f30-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54f30-209">size</span><span class="sxs-lookup"><span data-stu-id="54f30-209">size</span></span>|<span data-ttu-id="54f30-210">Int64</span><span class="sxs-lookup"><span data-stu-id="54f30-210">Int64</span></span>|<span data-ttu-id="54f30-211">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="54f30-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="54f30-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="54f30-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="54f30-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="54f30-213">applicableArchitectures</span></span>|[<span data-ttu-id="54f30-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="54f30-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="54f30-215">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="54f30-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="54f30-216">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="54f30-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="54f30-217">identityName</span><span class="sxs-lookup"><span data-stu-id="54f30-217">identityName</span></span>|<span data-ttu-id="54f30-218">String</span><span class="sxs-lookup"><span data-stu-id="54f30-218">String</span></span>|<span data-ttu-id="54f30-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="54f30-219">The Identity Name.</span></span>|
|<span data-ttu-id="54f30-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="54f30-220">identityPublisherHash</span></span>|<span data-ttu-id="54f30-221">String</span><span class="sxs-lookup"><span data-stu-id="54f30-221">String</span></span>|<span data-ttu-id="54f30-222">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="54f30-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="54f30-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="54f30-223">identityResourceIdentifier</span></span>|<span data-ttu-id="54f30-224">String</span><span class="sxs-lookup"><span data-stu-id="54f30-224">String</span></span>|<span data-ttu-id="54f30-225">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="54f30-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="54f30-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54f30-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="54f30-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54f30-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="54f30-228">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="54f30-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="54f30-229">Фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="54f30-229">phoneProductIdentifier</span></span>|<span data-ttu-id="54f30-230">String</span><span class="sxs-lookup"><span data-stu-id="54f30-230">String</span></span>|<span data-ttu-id="54f30-231">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="54f30-231">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="54f30-232">Фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="54f30-232">phonePublisherId</span></span>|<span data-ttu-id="54f30-233">String</span><span class="sxs-lookup"><span data-stu-id="54f30-233">String</span></span>|<span data-ttu-id="54f30-234">Идентификатор издателя телефона.</span><span class="sxs-lookup"><span data-stu-id="54f30-234">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="54f30-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="54f30-235">identityVersion</span></span>|<span data-ttu-id="54f30-236">String</span><span class="sxs-lookup"><span data-stu-id="54f30-236">String</span></span>|<span data-ttu-id="54f30-237">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="54f30-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="54f30-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="54f30-238">Response</span></span>
<span data-ttu-id="54f30-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54f30-239">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54f30-240">Пример</span><span class="sxs-lookup"><span data-stu-id="54f30-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="54f30-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="54f30-241">Request</span></span>
<span data-ttu-id="54f30-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54f30-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1440

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
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="54f30-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="54f30-243">Response</span></span>
<span data-ttu-id="54f30-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54f30-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1612

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
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




