# <a name="get-settings"></a><span data-ttu-id="88ab0-101">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="88ab0-101">Get settings</span></span>

<span data-ttu-id="88ab0-102">Чтение объекта [Параметры](../resources/user_settings.md) пользователей и организаций.</span><span class="sxs-lookup"><span data-stu-id="88ab0-102">Read the user and organization [settings](../resources/user_settings.md) object.</span></span>
<span data-ttu-id="88ab0-103">Чтобы узнать, как обновить свойства объекта [параметров](../resources/user_settings.md) , обратитесь к разделу [Изменение параметров пользователей](user_update_settings.md).</span><span class="sxs-lookup"><span data-stu-id="88ab0-103">To learn how to update the properties of the [settings](../resources/user_settings.md) object, see [update user settings](user_update_settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="88ab0-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88ab0-104">Permissions</span></span>

<span data-ttu-id="88ab0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="88ab0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88ab0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88ab0-107">Permission type</span></span>      | <span data-ttu-id="88ab0-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88ab0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88ab0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88ab0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="88ab0-110">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ab0-110">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="88ab0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88ab0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88ab0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88ab0-112">Not supported.</span></span>    |
|<span data-ttu-id="88ab0-113">Для приложения</span><span class="sxs-lookup"><span data-stu-id="88ab0-113">Application</span></span> | <span data-ttu-id="88ab0-114">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ab0-114">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88ab0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88ab0-115">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="88ab0-116">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="88ab0-116">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="88ab0-117">[Для получения дополнительных сведений см.](../../../concepts/permissions_reference.md)</span><span class="sxs-lookup"><span data-stu-id="88ab0-117">To learn more, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="88ab0-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88ab0-118">Request body</span></span>

<span data-ttu-id="88ab0-119">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88ab0-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88ab0-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="88ab0-120">Response</span></span>

<span data-ttu-id="88ab0-121">Успешно завершена, этот метод возвращает `200 OK` объект [параметров пользователя](../resources/user_settings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="88ab0-121">If successful, this method returns a `200 OK` response code and [user settings](../resources/user_settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88ab0-122">Пример</span><span class="sxs-lookup"><span data-stu-id="88ab0-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="88ab0-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="88ab0-123">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="88ab0-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="88ab0-124">Response</span></span>

<span data-ttu-id="88ab0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="88ab0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

