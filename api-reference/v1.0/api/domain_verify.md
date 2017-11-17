# <a name="domain-verify"></a><span data-ttu-id="fb25f-101">domain: verify</span><span class="sxs-lookup"><span data-stu-id="fb25f-101">domain: verify</span></span>

<span data-ttu-id="fb25f-102">Проверка права собственности на домен.</span><span class="sxs-lookup"><span data-stu-id="fb25f-102">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="fb25f-p101">**Важно!** Применяется только к непроверенному домену. Для непроверенного домена свойство isVerified объекта [domain](../resources/domain.md) будет иметь значение false.</span><span class="sxs-lookup"><span data-stu-id="fb25f-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb25f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb25f-105">Permissions</span></span>

<span data-ttu-id="fb25f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb25f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="fb25f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb25f-108">Permission type</span></span>      | <span data-ttu-id="fb25f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb25f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb25f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb25f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb25f-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb25f-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="fb25f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb25f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb25f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb25f-113">Not supported.</span></span>    |
|<span data-ttu-id="fb25f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb25f-114">Application</span></span> | <span data-ttu-id="fb25f-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb25f-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb25f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb25f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="fb25f-117">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="fb25f-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb25f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb25f-118">Request headers</span></span>

| <span data-ttu-id="fb25f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fb25f-119">Name</span></span>       | <span data-ttu-id="fb25f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fb25f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb25f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb25f-121">Authorization</span></span>  | <span data-ttu-id="fb25f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb25f-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="fb25f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb25f-124">Content-Type</span></span>  | <span data-ttu-id="fb25f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb25f-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb25f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb25f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fb25f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb25f-127">Response</span></span>

<span data-ttu-id="fb25f-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fb25f-128">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb25f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fb25f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb25f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb25f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="fb25f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb25f-131">Response</span></span>
<span data-ttu-id="fb25f-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb25f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->