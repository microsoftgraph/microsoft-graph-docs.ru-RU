# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="ca2ac-101">Работа с пользователями в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca2ac-101">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="ca2ac-102">Вы можете использовать Microsoft Graph для создания привлекательных приложений, учитывающих пользователей, их связи с другими пользователями и группами, а также почту, календарь и файлы.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-102">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="ca2ac-103">Вы можете получить доступ к [пользователям](user.md) через Microsoft Graph двумя указанными ниже способами.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-103">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="ca2ac-104">По идентификатору пользователя (`/users/{id | userPrincipalName}`).</span><span class="sxs-lookup"><span data-stu-id="ca2ac-104">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="ca2ac-105">С помощью псевдонима `/me` (который совпадает с `/users/{signed-in user's id}`) для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-105">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="ca2ac-106">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca2ac-106">Authorization</span></span>

<span data-ttu-id="ca2ac-p101">Для операций доступа к пользователям необходимо одно из указанных ниже [разрешений](https://developer.microsoft.com/graph/docs/authorization/permission_scopes). Первые три разрешения могут быть предоставлены приложению пользователем. Остальные разрешения могут быть предоставлены приложению администратором.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="ca2ac-110">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ca2ac-110">User.ReadBasic.All</span></span>
- <span data-ttu-id="ca2ac-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="ca2ac-111">User.Read</span></span>
- <span data-ttu-id="ca2ac-112">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca2ac-112">User.ReadWrite</span></span>
- <span data-ttu-id="ca2ac-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca2ac-113">User.Read.All</span></span>
- <span data-ttu-id="ca2ac-114">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2ac-114">User.ReadWrite.All</span></span>
- <span data-ttu-id="ca2ac-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca2ac-115">Directory.Read.All</span></span>
- <span data-ttu-id="ca2ac-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2ac-116">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="ca2ac-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca2ac-117">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="ca2ac-118">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="ca2ac-118">Common properties</span></span>

<span data-ttu-id="ca2ac-119">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении пользователя или выводе списка пользователей.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-119">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="ca2ac-120">Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-120">These are a subset of all available properties.</span></span> <span data-ttu-id="ca2ac-121">Чтобы получить дополнительные свойства пользователя, используйте параметр запроса `$select`.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-121">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="ca2ac-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca2ac-122">Property</span></span> |<span data-ttu-id="ca2ac-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2ac-123">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="ca2ac-124">id</span><span class="sxs-lookup"><span data-stu-id="ca2ac-124">id</span></span> | <span data-ttu-id="ca2ac-125">Уникальный идентификатор для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-125">The unique identifier for the user.</span></span>|
|<span data-ttu-id="ca2ac-126">businessPhones</span><span class="sxs-lookup"><span data-stu-id="ca2ac-126">businessPhones</span></span> | <span data-ttu-id="ca2ac-127">Номера телефонов пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-127">The user's phone numbers.</span></span>|
|<span data-ttu-id="ca2ac-128">displayName</span><span class="sxs-lookup"><span data-stu-id="ca2ac-128">displayName</span></span> | <span data-ttu-id="ca2ac-129">Имя, отображаемое в адресной книге, для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-129">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="ca2ac-130">givenName</span><span class="sxs-lookup"><span data-stu-id="ca2ac-130">givenName</span></span>| <span data-ttu-id="ca2ac-131">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-131">The first name of the user.</span></span> |
|<span data-ttu-id="ca2ac-132">jobTitle</span><span class="sxs-lookup"><span data-stu-id="ca2ac-132">jobTitle</span></span> | <span data-ttu-id="ca2ac-133">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-133">The user's job title.</span></span>|
|<span data-ttu-id="ca2ac-134">mail</span><span class="sxs-lookup"><span data-stu-id="ca2ac-134">mail</span></span>| <span data-ttu-id="ca2ac-135">Электронный адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-135">The user's email address.</span></span> |
|<span data-ttu-id="ca2ac-136">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="ca2ac-136">mobilePhone</span></span> | <span data-ttu-id="ca2ac-137">Номер мобильного телефона пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-137">The user's cellphone number.</span></span>|
|<span data-ttu-id="ca2ac-138">officeLocation</span><span class="sxs-lookup"><span data-stu-id="ca2ac-138">officeLocation</span></span> | <span data-ttu-id="ca2ac-139">Физическое расположение офиса пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-139">The user's physical office location.</span></span>|
|<span data-ttu-id="ca2ac-140">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="ca2ac-140">preferredLanguage</span></span> | <span data-ttu-id="ca2ac-141">Предпочитаемый язык пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-141">The user's language of preference.</span></span>|
|<span data-ttu-id="ca2ac-142">surname</span><span class="sxs-lookup"><span data-stu-id="ca2ac-142">surname</span></span>| <span data-ttu-id="ca2ac-143">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-143">The last name of the user.</span></span> |
|<span data-ttu-id="ca2ac-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ca2ac-144">userPrincipalName</span></span>| <span data-ttu-id="ca2ac-145">Имя участника-пользователя для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-145">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="ca2ac-146">Дополнительные сведения и список всех свойств см. в статье об объекте [user](user.md).</span><span class="sxs-lookup"><span data-stu-id="ca2ac-146">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="ca2ac-147">Стандартные действия</span><span class="sxs-lookup"><span data-stu-id="ca2ac-147">Common operations</span></span>

> <span data-ttu-id="ca2ac-148">**Примечание.** Для выполнения некоторых из этих операций необходимы дополнительные разрешения.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-148">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="ca2ac-149">Путь</span><span class="sxs-lookup"><span data-stu-id="ca2ac-149">Path</span></span>    | <span data-ttu-id="ca2ac-150">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2ac-150">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user_list.md) | <span data-ttu-id="ca2ac-151">Вывод списка пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-151">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user_get.md) | <span data-ttu-id="ca2ac-152">Получение определенного пользователя по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-152">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto_get.md)| <span data-ttu-id="ca2ac-153">Получение фотографии профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-153">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user_list_manager.md) | <span data-ttu-id="ca2ac-154">Получение сведений о руководителе пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-154">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user_list_messages.md)| <span data-ttu-id="ca2ac-155">Вывод списка электронных писем пользователя в его основном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-155">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user_list_events.md) | <span data-ttu-id="ca2ac-156">Вывод списка предстоящих событий пользователя из его календаря.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-156">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive_get.md)| <span data-ttu-id="ca2ac-157">Получение хранилища файлов OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-157">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user_list_memberof.md)| <span data-ttu-id="ca2ac-158">Вывод списка групп, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="ca2ac-158">Lists the groups that the user is a member of.</span></span> |
