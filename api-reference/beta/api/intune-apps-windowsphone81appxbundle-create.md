---
title: Создание windowsPhone81AppXBundle
description: Создание нового объекта windowsPhone81AppXBundle.
ms.openlocfilehash: 1df7a11bedf52d8c0ab685e786beb6b961e9f4dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081918"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="99b81-103">Создание windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="99b81-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="99b81-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99b81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99b81-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99b81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99b81-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99b81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99b81-107">Создание нового объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="99b81-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99b81-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="99b81-108">Prerequisites</span></span>
<span data-ttu-id="99b81-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99b81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99b81-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99b81-111">Permission type</span></span>|<span data-ttu-id="99b81-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99b81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99b81-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99b81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99b81-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b81-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99b81-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99b81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99b81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99b81-116">Not supported.</span></span>|
|<span data-ttu-id="99b81-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99b81-117">Application</span></span>|<span data-ttu-id="99b81-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99b81-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99b81-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99b81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="99b81-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99b81-120">Request headers</span></span>
|<span data-ttu-id="99b81-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99b81-121">Header</span></span>|<span data-ttu-id="99b81-122">Значение</span><span class="sxs-lookup"><span data-stu-id="99b81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99b81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99b81-123">Authorization</span></span>|<span data-ttu-id="99b81-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="99b81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99b81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99b81-125">Accept</span></span>|<span data-ttu-id="99b81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99b81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99b81-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99b81-127">Request body</span></span>
<span data-ttu-id="99b81-128">В тексте запроса укажите представление JSON для объекта windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="99b81-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="99b81-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="99b81-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="99b81-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="99b81-130">Property</span></span>|<span data-ttu-id="99b81-131">Тип</span><span class="sxs-lookup"><span data-stu-id="99b81-131">Type</span></span>|<span data-ttu-id="99b81-132">Описание</span><span class="sxs-lookup"><span data-stu-id="99b81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b81-133">id</span><span class="sxs-lookup"><span data-stu-id="99b81-133">id</span></span>|<span data-ttu-id="99b81-134">String</span><span class="sxs-lookup"><span data-stu-id="99b81-134">String</span></span>|<span data-ttu-id="99b81-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99b81-135">Key of the entity.</span></span> <span data-ttu-id="99b81-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-137">displayName</span><span class="sxs-lookup"><span data-stu-id="99b81-137">displayName</span></span>|<span data-ttu-id="99b81-138">String</span><span class="sxs-lookup"><span data-stu-id="99b81-138">String</span></span>|<span data-ttu-id="99b81-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="99b81-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="99b81-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-141">описание</span><span class="sxs-lookup"><span data-stu-id="99b81-141">description</span></span>|<span data-ttu-id="99b81-142">String</span><span class="sxs-lookup"><span data-stu-id="99b81-142">String</span></span>|<span data-ttu-id="99b81-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-143">The description of the app.</span></span> <span data-ttu-id="99b81-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-145">publisher</span><span class="sxs-lookup"><span data-stu-id="99b81-145">publisher</span></span>|<span data-ttu-id="99b81-146">String</span><span class="sxs-lookup"><span data-stu-id="99b81-146">String</span></span>|<span data-ttu-id="99b81-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-147">The publisher of the app.</span></span> <span data-ttu-id="99b81-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="99b81-149">largeIcon</span></span>|[<span data-ttu-id="99b81-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99b81-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99b81-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="99b81-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="99b81-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99b81-153">createdDateTime</span></span>|<span data-ttu-id="99b81-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b81-154">DateTimeOffset</span></span>|<span data-ttu-id="99b81-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-155">The date and time the app was created.</span></span> <span data-ttu-id="99b81-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99b81-157">lastModifiedDateTime</span></span>|<span data-ttu-id="99b81-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b81-158">DateTimeOffset</span></span>|<span data-ttu-id="99b81-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-159">The date and time the app was last modified.</span></span> <span data-ttu-id="99b81-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="99b81-161">isFeatured</span></span>|<span data-ttu-id="99b81-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="99b81-162">Boolean</span></span>|<span data-ttu-id="99b81-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="99b81-164">privacyInformationUrl</span></span>|<span data-ttu-id="99b81-165">String</span><span class="sxs-lookup"><span data-stu-id="99b81-165">String</span></span>|<span data-ttu-id="99b81-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="99b81-166">The privacy statement Url.</span></span> <span data-ttu-id="99b81-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="99b81-168">informationUrl</span></span>|<span data-ttu-id="99b81-169">String</span><span class="sxs-lookup"><span data-stu-id="99b81-169">String</span></span>|<span data-ttu-id="99b81-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="99b81-170">The more information Url.</span></span> <span data-ttu-id="99b81-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-172">owner</span><span class="sxs-lookup"><span data-stu-id="99b81-172">owner</span></span>|<span data-ttu-id="99b81-173">String</span><span class="sxs-lookup"><span data-stu-id="99b81-173">String</span></span>|<span data-ttu-id="99b81-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-174">The owner of the app.</span></span> <span data-ttu-id="99b81-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-176">developer</span><span class="sxs-lookup"><span data-stu-id="99b81-176">developer</span></span>|<span data-ttu-id="99b81-177">String</span><span class="sxs-lookup"><span data-stu-id="99b81-177">String</span></span>|<span data-ttu-id="99b81-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-178">The developer of the app.</span></span> <span data-ttu-id="99b81-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-180">notes</span><span class="sxs-lookup"><span data-stu-id="99b81-180">notes</span></span>|<span data-ttu-id="99b81-181">String</span><span class="sxs-lookup"><span data-stu-id="99b81-181">String</span></span>|<span data-ttu-id="99b81-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="99b81-182">Notes for the app.</span></span> <span data-ttu-id="99b81-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="99b81-184">uploadState</span></span>|<span data-ttu-id="99b81-185">Int32</span><span class="sxs-lookup"><span data-stu-id="99b81-185">Int32</span></span>|<span data-ttu-id="99b81-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="99b81-186">The upload state.</span></span> <span data-ttu-id="99b81-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b81-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="99b81-188">publishingState</span></span>|[<span data-ttu-id="99b81-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="99b81-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="99b81-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-190">The publishing state for the app.</span></span> <span data-ttu-id="99b81-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="99b81-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="99b81-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="99b81-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="99b81-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="99b81-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="99b81-194">committedContentVersion</span></span>|<span data-ttu-id="99b81-195">String</span><span class="sxs-lookup"><span data-stu-id="99b81-195">String</span></span>|<span data-ttu-id="99b81-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="99b81-196">The internal committed content version.</span></span> <span data-ttu-id="99b81-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="99b81-198">fileName</span><span class="sxs-lookup"><span data-stu-id="99b81-198">fileName</span></span>|<span data-ttu-id="99b81-199">String</span><span class="sxs-lookup"><span data-stu-id="99b81-199">String</span></span>|<span data-ttu-id="99b81-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="99b81-200">The name of the main Lob application file.</span></span> <span data-ttu-id="99b81-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="99b81-202">size</span><span class="sxs-lookup"><span data-stu-id="99b81-202">size</span></span>|<span data-ttu-id="99b81-203">Int64</span><span class="sxs-lookup"><span data-stu-id="99b81-203">Int64</span></span>|<span data-ttu-id="99b81-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="99b81-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="99b81-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="99b81-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="99b81-206">applicableArchitectures</span></span>|[<span data-ttu-id="99b81-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="99b81-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="99b81-208">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="99b81-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="99b81-209">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="99b81-209">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="99b81-210">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="99b81-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="99b81-211">identityName</span><span class="sxs-lookup"><span data-stu-id="99b81-211">identityName</span></span>|<span data-ttu-id="99b81-212">String</span><span class="sxs-lookup"><span data-stu-id="99b81-212">String</span></span>|<span data-ttu-id="99b81-213">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="99b81-213">The Identity Name.</span></span> <span data-ttu-id="99b81-214">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="99b81-214">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="99b81-215">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="99b81-215">identityPublisherHash</span></span>|<span data-ttu-id="99b81-216">String</span><span class="sxs-lookup"><span data-stu-id="99b81-216">String</span></span>|<span data-ttu-id="99b81-217">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="99b81-217">The Identity Publisher Hash.</span></span> <span data-ttu-id="99b81-218">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="99b81-218">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="99b81-219">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="99b81-219">identityResourceIdentifier</span></span>|<span data-ttu-id="99b81-220">String</span><span class="sxs-lookup"><span data-stu-id="99b81-220">String</span></span>|<span data-ttu-id="99b81-221">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="99b81-221">The Identity Resource Identifier.</span></span> <span data-ttu-id="99b81-222">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="99b81-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="99b81-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="99b81-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="99b81-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="99b81-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="99b81-225">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="99b81-225">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="99b81-226">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="99b81-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="99b81-227">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="99b81-227">phoneProductIdentifier</span></span>|<span data-ttu-id="99b81-228">String</span><span class="sxs-lookup"><span data-stu-id="99b81-228">String</span></span>|<span data-ttu-id="99b81-229">Идентификатор продукта телефона.</span><span class="sxs-lookup"><span data-stu-id="99b81-229">The Phone Product Identifier.</span></span> <span data-ttu-id="99b81-230">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="99b81-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="99b81-231">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="99b81-231">phonePublisherId</span></span>|<span data-ttu-id="99b81-232">String</span><span class="sxs-lookup"><span data-stu-id="99b81-232">String</span></span>|<span data-ttu-id="99b81-233">Идентификатор издателя телефона наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="99b81-233">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="99b81-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="99b81-234">identityVersion</span></span>|<span data-ttu-id="99b81-235">String</span><span class="sxs-lookup"><span data-stu-id="99b81-235">String</span></span>|<span data-ttu-id="99b81-236">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="99b81-236">The identity version.</span></span> <span data-ttu-id="99b81-237">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="99b81-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="99b81-238">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="99b81-238">appXPackageInformationList</span></span>|<span data-ttu-id="99b81-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="99b81-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="99b81-240">Список AppX сведения о пакете.</span><span class="sxs-lookup"><span data-stu-id="99b81-240">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="99b81-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="99b81-241">Response</span></span>
<span data-ttu-id="99b81-242">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="99b81-242">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99b81-243">Пример</span><span class="sxs-lookup"><span data-stu-id="99b81-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="99b81-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="99b81-244">Request</span></span>
<span data-ttu-id="99b81-245">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99b81-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2163

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="99b81-246">Ответ</span><span class="sxs-lookup"><span data-stu-id="99b81-246">Response</span></span>
<span data-ttu-id="99b81-p127">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="99b81-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2271

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```





