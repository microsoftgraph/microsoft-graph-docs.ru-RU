---
title: Create windowsMobileMSI
description: Создание объекта windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9e9ba8c10d80ea75799046b951678d34bf88a2d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966378"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="cc3c5-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="cc3c5-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="cc3c5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc3c5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc3c5-106">Создание объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc3c5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cc3c5-107">Prerequisites</span></span>
<span data-ttu-id="cc3c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc3c5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc3c5-110">Permission type</span></span>|<span data-ttu-id="cc3c5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc3c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc3c5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc3c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc3c5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cc3c5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc3c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc3c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-115">Not supported.</span></span>|
|<span data-ttu-id="cc3c5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc3c5-116">Application</span></span>|<span data-ttu-id="cc3c5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc3c5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc3c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cc3c5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc3c5-119">Request headers</span></span>
|<span data-ttu-id="cc3c5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc3c5-120">Header</span></span>|<span data-ttu-id="cc3c5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc3c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc3c5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc3c5-122">Authorization</span></span>|<span data-ttu-id="cc3c5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc3c5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cc3c5-124">Accept</span></span>|<span data-ttu-id="cc3c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc3c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc3c5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc3c5-126">Request body</span></span>
<span data-ttu-id="cc3c5-127">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="cc3c5-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="cc3c5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc3c5-129">Property</span></span>|<span data-ttu-id="cc3c5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cc3c5-130">Type</span></span>|<span data-ttu-id="cc3c5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cc3c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc3c5-132">id</span><span class="sxs-lookup"><span data-stu-id="cc3c5-132">id</span></span>|<span data-ttu-id="cc3c5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cc3c5-133">String</span></span>|<span data-ttu-id="cc3c5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-134">Key of the entity.</span></span> <span data-ttu-id="cc3c5-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cc3c5-136">displayName</span></span>|<span data-ttu-id="cc3c5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cc3c5-137">String</span></span>|<span data-ttu-id="cc3c5-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cc3c5-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-140">description</span><span class="sxs-lookup"><span data-stu-id="cc3c5-140">description</span></span>|<span data-ttu-id="cc3c5-141">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-141">String</span></span>|<span data-ttu-id="cc3c5-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-142">The description of the app.</span></span> <span data-ttu-id="cc3c5-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cc3c5-144">publisher</span></span>|<span data-ttu-id="cc3c5-145">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-145">String</span></span>|<span data-ttu-id="cc3c5-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-146">The publisher of the app.</span></span> <span data-ttu-id="cc3c5-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cc3c5-148">largeIcon</span></span>|[<span data-ttu-id="cc3c5-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cc3c5-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cc3c5-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cc3c5-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc3c5-152">createdDateTime</span></span>|<span data-ttu-id="cc3c5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc3c5-153">DateTimeOffset</span></span>|<span data-ttu-id="cc3c5-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-154">The date and time the app was created.</span></span> <span data-ttu-id="cc3c5-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc3c5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cc3c5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc3c5-157">DateTimeOffset</span></span>|<span data-ttu-id="cc3c5-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cc3c5-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cc3c5-160">isFeatured</span></span>|<span data-ttu-id="cc3c5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc3c5-161">Boolean</span></span>|<span data-ttu-id="cc3c5-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cc3c5-163">privacyInformationUrl</span></span>|<span data-ttu-id="cc3c5-164">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-164">String</span></span>|<span data-ttu-id="cc3c5-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-165">The privacy statement Url.</span></span> <span data-ttu-id="cc3c5-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cc3c5-167">informationUrl</span></span>|<span data-ttu-id="cc3c5-168">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-168">String</span></span>|<span data-ttu-id="cc3c5-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-169">The more information Url.</span></span> <span data-ttu-id="cc3c5-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-171">owner</span><span class="sxs-lookup"><span data-stu-id="cc3c5-171">owner</span></span>|<span data-ttu-id="cc3c5-172">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-172">String</span></span>|<span data-ttu-id="cc3c5-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-173">The owner of the app.</span></span> <span data-ttu-id="cc3c5-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-175">developer</span><span class="sxs-lookup"><span data-stu-id="cc3c5-175">developer</span></span>|<span data-ttu-id="cc3c5-176">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-176">String</span></span>|<span data-ttu-id="cc3c5-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-177">The developer of the app.</span></span> <span data-ttu-id="cc3c5-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-179">notes</span><span class="sxs-lookup"><span data-stu-id="cc3c5-179">notes</span></span>|<span data-ttu-id="cc3c5-180">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-180">String</span></span>|<span data-ttu-id="cc3c5-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-181">Notes for the app.</span></span> <span data-ttu-id="cc3c5-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cc3c5-183">uploadState</span></span>|<span data-ttu-id="cc3c5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cc3c5-184">Int32</span></span>|<span data-ttu-id="cc3c5-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-185">The upload state.</span></span> <span data-ttu-id="cc3c5-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cc3c5-187">publishingState</span></span>|[<span data-ttu-id="cc3c5-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="cc3c5-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cc3c5-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-189">The publishing state for the app.</span></span> <span data-ttu-id="cc3c5-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cc3c5-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cc3c5-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cc3c5-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cc3c5-193">isAssigned</span></span>|<span data-ttu-id="cc3c5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc3c5-194">Boolean</span></span>|<span data-ttu-id="cc3c5-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cc3c5-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc3c5-197">roleScopeTagIds</span></span>|<span data-ttu-id="cc3c5-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cc3c5-198">String collection</span></span>|<span data-ttu-id="cc3c5-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cc3c5-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc3c5-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cc3c5-201">committedContentVersion</span></span>|<span data-ttu-id="cc3c5-202">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-202">String</span></span>|<span data-ttu-id="cc3c5-203">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-203">The internal committed content version.</span></span> <span data-ttu-id="cc3c5-204">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc3c5-205">fileName</span><span class="sxs-lookup"><span data-stu-id="cc3c5-205">fileName</span></span>|<span data-ttu-id="cc3c5-206">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-206">String</span></span>|<span data-ttu-id="cc3c5-207">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-207">The name of the main Lob application file.</span></span> <span data-ttu-id="cc3c5-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc3c5-209">size</span><span class="sxs-lookup"><span data-stu-id="cc3c5-209">size</span></span>|<span data-ttu-id="cc3c5-210">Int64</span><span class="sxs-lookup"><span data-stu-id="cc3c5-210">Int64</span></span>|<span data-ttu-id="cc3c5-211">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="cc3c5-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc3c5-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc3c5-213">commandLine</span><span class="sxs-lookup"><span data-stu-id="cc3c5-213">commandLine</span></span>|<span data-ttu-id="cc3c5-214">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-214">String</span></span>|<span data-ttu-id="cc3c5-215">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-215">The command line.</span></span>|
|<span data-ttu-id="cc3c5-216">productCode</span><span class="sxs-lookup"><span data-stu-id="cc3c5-216">productCode</span></span>|<span data-ttu-id="cc3c5-217">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-217">String</span></span>|<span data-ttu-id="cc3c5-218">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-218">The product code.</span></span>|
|<span data-ttu-id="cc3c5-219">productVersion</span><span class="sxs-lookup"><span data-stu-id="cc3c5-219">productVersion</span></span>|<span data-ttu-id="cc3c5-220">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-220">String</span></span>|<span data-ttu-id="cc3c5-221">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-221">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cc3c5-222">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="cc3c5-222">ignoreVersionDetection</span></span>|<span data-ttu-id="cc3c5-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc3c5-223">Boolean</span></span>|<span data-ttu-id="cc3c5-224">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-224">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="cc3c5-225">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-225">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="cc3c5-226">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cc3c5-226">identityVersion</span></span>|<span data-ttu-id="cc3c5-227">String</span><span class="sxs-lookup"><span data-stu-id="cc3c5-227">String</span></span>|<span data-ttu-id="cc3c5-228">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-228">The identity version.</span></span>|
|<span data-ttu-id="cc3c5-229">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="cc3c5-229">useDeviceContext</span></span>|<span data-ttu-id="cc3c5-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc3c5-230">Boolean</span></span>|<span data-ttu-id="cc3c5-231">Указывает, следует ли установить MSI с двойным режимом в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-231">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="cc3c5-232">Если задано значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-232">If true, app will be installed for all users.</span></span> <span data-ttu-id="cc3c5-233">Если задано значение false, приложение будет установлено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-233">If false, app will be installed per-user.</span></span> <span data-ttu-id="cc3c5-234">Если значение равно null, служба будет использовать стандартный контекст установки пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-234">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="cc3c5-235">В случае с двойным режимом MSI это значение по умолчанию будет иметь значение "на пользователя".</span><span class="sxs-lookup"><span data-stu-id="cc3c5-235">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="cc3c5-236">Не может быть задано для приложений с несдвоенным режимом.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-236">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="cc3c5-237">После первоначального создания приложения его невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-237">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="cc3c5-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc3c5-238">Response</span></span>
<span data-ttu-id="cc3c5-239">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-239">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc3c5-240">Пример</span><span class="sxs-lookup"><span data-stu-id="cc3c5-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc3c5-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc3c5-241">Request</span></span>
<span data-ttu-id="cc3c5-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="cc3c5-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc3c5-243">Response</span></span>
<span data-ttu-id="cc3c5-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




